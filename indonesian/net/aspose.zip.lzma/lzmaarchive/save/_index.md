---
title: LzmaArchive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzmaArchive metode. Menyimpan arsip lzma ke aliran yang disediakan.
type: docs
weight: 40
url: /id/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

Menyimpan arsip lzma ke aliran yang disediakan.

```csharp
public void Save(Stream output)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *output* tidak mendukung pencarian. |
| ArgumentNullException | *output* adalah nol. |

### Perkataan

*output* harus dapat dicari.

### Contoh

```csharp
using (FileStream lzmaFile = File.Open("archive.lzma", FileMode.Create))
{
    using (var archive = new LzmaArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzmaFile);
     }
}
```

### Lihat juga

* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Menyimpan arsip lzma ke file tujuan yang disediakan.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | FileInfo | FileInfo yang akan dibuka sebagai aliran tujuan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk membuka*destination*. |
| ArgumentException | Jalur file kosong atau hanya berisi spasi putih. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau direktori. |
| ArgumentNullException | *destination* adalah nol. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, seperti berada di drive yang belum dipetakan. |
| IOException | File sudah terbuka. |

### Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### Lihat juga

* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Menyimpan arsip lzma ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*destinationFileName* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*destinationFileName* ditolak. |
| PathTooLongException | Yang ditentukan*destinationFileName*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*destinationFileName* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### Lihat juga

* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)


