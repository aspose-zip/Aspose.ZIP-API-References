---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchive metode. Buat satu entri dalam arsip.
type: docs
weight: 50
url: /id/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) barang. |

### Nilai Pengembalian

Contoh entri Seven Zip.

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

Buat arsip dengan entri yang dienkripsi masing-masing dengan kata sandi yang berbeda.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) barang. |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Pengembalian

Instance entri SevenZip.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Keduanya*source* Dan*fileInfo* adalah nol atau*source*adalah nol dan*fileInfo* singkatan dari direktori. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*fileInfo* parameter tidak mempengaruhi nama entri.

*fileInfo* dapat merujuk keDirectoryInfo jika entri adalah direktori.

### Contoh

Buat arsip dengan entri terenkripsi terkompresi LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) barang. |

### Nilai Pengembalian

Contoh entri zip.

### Contoh

Buat arsip 7z dengan kompresi LZMA2 dan enkripsi semua entri.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Nama file baru yang sepenuhnya memenuhi syarat, atau nama file relatif yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk ditambahkan[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) barang. |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)


