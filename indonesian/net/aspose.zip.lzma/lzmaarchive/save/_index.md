---
title: "LzmaArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode LzmaArchive. Menyimpan arsip lzma ke aliran yang disediakan"
type: docs
weight: 50
url: /id/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

Menyimpan arsip lzma ke stream yang diberikan.

```csharp
public void Save(Stream output)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *output* tidak mendukung pencarian. |
| ArgumentNullException | *output* adalah null. |

## Catatan

*output* must be seekable.

## Contoh

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

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Menyimpan arsip lzma ke file tujuan yang diberikan.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | FileInfo | FileInfo, yang akan dibuka sebagai aliran tujuan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk membuka *destination*. |
| ArgumentException | Path file kosong atau hanya berisi spasi. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau merupakan direktori. |
| ArgumentNullException | *destination* bernilai null. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |

## Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Menyimpan arsip lzma ke file tujuan yang diberikan.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *destinationFileName* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *destinationFileName* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *destinationFileName* ditolak. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *destinationFileName* berisi tanda titik dua (:) di tengah string. |
| FileNotFoundException | File yang ditentukan dalam *path* tidak ditemukan. |
| IOException | Terjadi kesalahan I/O saat membuka file. |

## Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


