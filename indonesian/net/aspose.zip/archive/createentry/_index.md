---
title: "Archive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Archive. Membuat satu entri di dalam arsip."
type: docs
weight: 60
url: /id/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_4}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Nama lengkap dari file baru, atau nama file relatif yang akan dikompres. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan dalam parameter *path* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately* maka akan diblokir sampai arsip disimpan.

## Contoh

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

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| InvalidOperationException | Dilemparkan ketika penambahan entri tidak valid karena keadaan arsip saat ini. |

## Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file yang akan dikompresi. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* bersifat read-only atau merupakan direktori. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| InvalidOperationException | Dilemparkan ketika penambahan entri tidak valid karena keadaan arsip saat ini. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately* maka akan diblokir sampai arsip disimpan.

## Contoh

Susun arsip dengan entri yang dienkripsi menggunakan metode enkripsi dan kata sandi yang berbeda masing‑masing.

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

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_3}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang ditambahkan. |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Baik *source* maupun *fileInfo* bernilai null atau *source* null dan *fileInfo* mengacu pada direktori. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Contoh

Susun arsip dengan entri terenkripsi.

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

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, ArchiveEntrySettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public ArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| streamProvider | Func`1 | Metode yang menyediakan aliran masukan untuk entri. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| ArgumentException | Dilempar ketika *name* bernilai null atau kosong, atau *streamProvider* bernilai null. |
| InvalidOperationException | Dilempar ketika arsip tidak mendukung penambahan entri. |

## Catatan

Metode ini untuk .NET Framework 4.0 ke atas dan untuk versi .NET Standard 2.0 ke atas.

## Contoh

Susun arsip dengan entri terenkripsi.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")))); 
        archive.Save(zipFile);
    }
}
```

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


