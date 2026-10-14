---
title: "ZArchive.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ZArchive. Mengekstrak arsip Z ke sebuah stream"
type: docs
weight: 30
url: /id/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Mengekstrak arsip Z ke sebuah stream.

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
| InvalidDataException | Data tidak dapat didekompresi. |

## Contoh

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

### Lihat Juga

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Mengekstrak arsip Z ke sebuah file.

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
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk membuka *fileInfo*. |
| ArgumentException | Path file kosong atau hanya berisi spasi. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau merupakan direktori. |
| ArgumentNullException | *fileInfo* bernilai null. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| InvalidDataException | Data tidak dapat didekompresi. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Contoh

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Lihat Juga

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Mengekstrak arsip Z ke sebuah file berdasarkan path.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan menyimpan data terdekompresi. |

### Nilai Kembalian

Info tentang file yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| InvalidDataException | Data tidak dapat didekompresi. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |

## Contoh

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Lihat Juga

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


