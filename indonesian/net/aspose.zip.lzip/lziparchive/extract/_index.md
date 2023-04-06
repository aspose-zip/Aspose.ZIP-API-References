---
title: LzipArchive.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzipArchive metode. Mengekstrak arsip lzip ke aliran.
type: docs
weight: 40
url: /id/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Mengekstrak arsip lzip ke aliran.

```csharp
public void Extract(Stream destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Stream untuk menyimpan data yang didekompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Tajuk arsip dan informasi layanan tidak dibaca. |
| InvalidDataException | Kesalahan dalam data di header atau checksum. |
| ArgumentNullException | Aliran tujuan adalah nol. |
| ArgumentException | Aliran tujuan tidak mendukung penulisan. |

### Contoh

```csharp
using (FileStream sourceLzipFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new LzipArchive(sourceLzipFile))
        {
               archive.Extract(extractedFile);
           }
       }
}
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Mengekstrak arsip lzip ke file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo untuk menyimpan data yang didekompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Tajuk arsip dan informasi layanan tidak dibaca. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk membuka*fileInfo*. |
| ArgumentException | Jalur file kosong atau hanya berisi spasi putih. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau direktori. |
| ArgumentNullException | *fileInfo* adalah nol. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, seperti berada di drive yang belum dipetakan. |
| IOException | File sudah terbuka. |

### Contoh

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Mengekstrak arsip lzip ke file dengan jalur.

```csharp
public void Extract(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file yang akan menyimpan data yang didekompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Tajuk arsip dan informasi layanan tidak dibaca. |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)


