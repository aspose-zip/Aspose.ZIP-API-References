---
title: "LzipArchive.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode LzipArchive. Mengekstrak arsip lzip ke aliran"
type: docs
weight: 50
url: /id/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Mengekstrak arsip lzip ke sebuah aliran.

```csharp
public void Extract(Stream destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Aliran untuk menyimpan data yang didekompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |
| InvalidDataException | Kesalahan data pada header atau checksum. |
| ArgumentNullException | Aliran tujuan bernilai null. |
| ArgumentException | Aliran tujuan tidak mendukung penulisan. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Contoh

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

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Mengekstrak arsip lzip ke sebuah file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo untuk menyimpan data yang telah didekompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk membuka *fileInfo*. |
| ArgumentException | Path file kosong atau hanya berisi spasi. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau merupakan direktori. |
| ArgumentNullException | *fileInfo* bernilai null. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Contoh

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Mengekstrak arsip lzip ke file berdasarkan jalur.

```csharp
public void Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan menyimpan data terdekompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |

## Contoh

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


