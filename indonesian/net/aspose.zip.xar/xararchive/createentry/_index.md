---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode XarArchive. Membuat satu entri dalam arsip"
type: docs
weight: 40
url: /id/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file atau folder yang akan dikompresi. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| compressionSettings | XarCompressionSettings | Pengaturan kompresi yang digunakan untuk item [`XarEntry`](../../xarentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Xar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *name* bernilai null. |
| ArgumentException | *name* kosong. |
| ArgumentNullException | *fileInfo* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Lihat Juga

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| sourcePath | String | Jalur ke file yang akan dikompres. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |
| compressionSettings | XarCompressionSettings | Pengaturan kompresi yang digunakan untuk item [`XarEntry`](../../xarentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Xar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourcePath* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *sourcePath* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. - atau - Nama file, sebagai bagian dari *name*, melebihi 100 simbol. |
| UnauthorizedAccessException | Akses ke file *sourcePath* ditolak. |
| PathTooLongException | *sourcePath* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. - atau - *name* terlalu panjang untuk xar. |
| NotSupportedException | File di *sourcePath* mengandung tanda titik dua (:) di tengah string. |
| InvalidOperationException | Tidak dapat memodifikasi arsip xar. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Nama entri hanya ditetapkan melalui parameter *name*. Nama file yang diberikan dalam parameter *sourcePath* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Lihat Juga

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| compressionSettings | XarCompressionSettings | Pengaturan kompresi yang digunakan untuk item [`XarEntry`](../../xarentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Xar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *name* bernilai null. |
| ArgumentNullException | *source* bernilai null. |
| ArgumentException | *name* kosong. |
| InvalidOperationException | Tidak dapat memodifikasi arsip xar. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Lihat Juga

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


