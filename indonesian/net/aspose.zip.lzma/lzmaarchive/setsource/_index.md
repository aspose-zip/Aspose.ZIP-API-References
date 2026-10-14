---
title: "LzmaArchive.SetSource"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode LzmaArchive. Mengatur konten yang akan dikompresi dalam arsip"
type: docs
weight: 60
url: /id/net/aspose.zip.lzma/lzmaarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Stream input untuk arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | Aliran *source* tidak dapat dicari. |

## Contoh

```csharp
using (var archive = new LzmaArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lzma");
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo, yang akan dibuka sebagai aliran masukan. |

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

## Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lzma");
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string sourcePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourcePath | String | Jalur ke file yang akan dibuka sebagai aliran masukan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *sourcePath* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Path *sourcePath* kosong, hanya berisi spasi putih, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *sourcePath* ditolak. |
| PathTooLongException | Path *sourcePath* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, path harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *sourcePath* mengandung tanda titik dua (:) di tengah string. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |

## Contoh

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lzma");
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


