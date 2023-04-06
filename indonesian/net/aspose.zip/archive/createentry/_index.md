---
title: Archive.CreateEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Buat satu entri dalam arsip.
type: docs
weight: 50
url: /id/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Nama file baru yang sepenuhnya memenuhi syarat, atau nama file relatif yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`ArchiveEntry`](../../archiveentry/) barang. |

### Nilai Pengembalian

Contoh entri zip.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*path* parameter tidak mempengaruhi nama entri.

Jika file segera dibuka dengan*openImmediately* parameter itu menjadi diblokir sampai arsip disimpan.

### Contoh

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Lihat juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`ArchiveEntry`](../../archiveentry/) barang. |

### Nilai Pengembalian

Contoh entri zip.

### Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Lihat juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`ArchiveEntry`](../../archiveentry/) barang. |

### Nilai Pengembalian

Contoh entri zip.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* bersifat read-only atau direktori. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, seperti berada di drive yang belum dipetakan. |
| IOException | File sudah terbuka. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*fileInfo* parameter tidak mempengaruhi nama entri.

Jika file segera dibuka dengan*openImmediately* parameter itu menjadi diblokir sampai arsip disimpan.

### Contoh

Buat arsip dengan entri yang dienkripsi dengan metode enkripsi dan kata sandi yang berbeda.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Lihat juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`ArchiveEntry`](../../archiveentry/) barang. |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Pengembalian

Contoh entri zip.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Keduanya*source* Dan*fileInfo* adalah nol atau*source*adalah nol dan*fileInfo* singkatan dari direktori. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*fileInfo* parameter tidak mempengaruhi nama entri.

*fileInfo* dapat merujuk keDirectoryInfo jika entri adalah direktori.

### Contoh

Buat arsip dengan entri terenkripsi.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Lihat juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


