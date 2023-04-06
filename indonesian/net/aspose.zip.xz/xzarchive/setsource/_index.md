---
title: XzArchive.SetSource
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzArchive metode. Mengatur konten yang akan dikompresi dalam arsip.
type: docs
weight: 50
url: /id/net/aspose.zip.xz/xzarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| source | Stream | Aliran input untuk arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Itu*source* aliran tidak dapat dicari. |

### Contoh

```csharp
using (var archive = new XzArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.xz");
}
```

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo yang akan dibuka sebagai input stream. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk membuka*fileInfo*. |
| ArgumentException | Jalur file kosong atau hanya berisi spasi putih. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau direktori. |
| ArgumentNullException | *fileInfo* adalah nol. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, seperti berada di drive yang belum dipetakan. |
| IOException | File sudah terbuka. |

### Contoh

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.xz");
}
```

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string sourcePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourcePath | String | Path ke file yang akan dibuka sebagai input stream. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourcePath* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*sourcePath* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*sourcePath* ditolak. |
| PathTooLongException | Yang ditentukan*sourcePath*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*sourcePath* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)


