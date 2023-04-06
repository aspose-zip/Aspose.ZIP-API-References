---
title: ZArchive.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: ZArchive metode. Mengekstrak arsip Z ke aliran.
type: docs
weight: 30
url: /id/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Mengekstrak arsip Z ke aliran.

```csharp
public void Extract(Stream destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Stream untuk menyimpan data yang didekompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidDataException | Data tidak dapat didekompresi. |

### Contoh

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Lihat juga

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Mengekstrak arsip Z ke file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo untuk menyimpan data yang didekompresi. |

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
| InvalidDataException | Data tidak dapat didekompresi. |

### Contoh

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Lihat juga

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Mengekstrak arsip Z ke file dengan jalur.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file yang akan menyimpan data yang didekompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |
| InvalidDataException | Data tidak dapat didekompresi. |

### Contoh

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Lihat juga

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)


