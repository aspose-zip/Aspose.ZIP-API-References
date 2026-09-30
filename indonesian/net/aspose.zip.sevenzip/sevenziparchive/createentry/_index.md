---
title: "SevenZipArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SevenZipArchive. Membuat satu entri di dalam arsip"
type: docs
weight: 50
url: /id/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file yang akan dikompresi. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang ditambahkan. Pengaturan kompresi individual diabaikan dalam kasus kompresi solid, lihat [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Nilai Kembalian

Instansi entri Seven Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* bersifat read-only atau merupakan direktori. |
| ArgumentException | *name* adalah null atau kosong. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately* maka akan diblokir sampai arsip disimpan.

## Contoh

Buat arsip dengan entri yang dienkripsi dengan kata sandi yang berbeda masing‑masing.

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

### Lihat Juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_3}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang ditambahkan. Pengaturan kompresi individual diabaikan dalam kasus kompresi solid, lihat [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Kembalian

Instansi entri SevenZip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Baik *source* maupun *fileInfo* bernilai null atau *source* null dan *fileInfo* mengacu pada direktori. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *name* adalah null atau kosong. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Contoh

Buat arsip dengan entri terenkripsi yang dikompresi LZMA2.

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

### Lihat Juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, SevenZipEntrySettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| streamProvider | Func`1 | Metode yang menyediakan aliran masukan untuk entri. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang ditambahkan. Pengaturan kompresi individual diabaikan dalam kasus kompresi solid, lihat [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Nilai Kembalian

Instansi entri SevenZip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip diinstansiasi untuk dekompresi |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *name* adalah null atau kosong. |

## Contoh

Buat arsip dengan entri terenkripsi yang dikompresi LZMA2.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
        archive.Save(sevenZipFile);
    }
}
```

### Lihat Juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang ditambahkan. Pengaturan kompresi individual diabaikan dalam kasus kompresi solid, lihat [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *name* adalah null atau kosong. |

## Contoh

Buat arsip 7z dengan kompresi LZMA2 dan enkripsi semua entri.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Lihat Juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_4}

Buat satu entri dalam arsip.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Nama lengkap dari file baru, atau nama file relatif yang akan dikompres. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang ditambahkan. Pengaturan kompresi individual diabaikan dalam kasus kompresi solid, lihat [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Nilai Kembalian

Instansi entri Zip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. - atau - *name* adalah null atau kosong. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan dalam parameter *path* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately* maka akan diblokir sampai arsip disimpan.

## Contoh

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

### Lihat Juga

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


