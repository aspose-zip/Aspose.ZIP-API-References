---
title: LzipArchive.SetSource
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzipArchive metode. Mengatur konten yang akan dikompresi dalam arsip.
type: docs
weight: 60
url: /id/net/aspose.zip.lzip/lziparchive/setsource/
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
using (var archive = new LzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz");

```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz");
}
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file yang akan dikompresi.. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz");
}
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)


