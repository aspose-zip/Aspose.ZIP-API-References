---
title: "LzipArchive.SetSource"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode LzipArchive. Mengatur konten yang akan dikompresi dalam arsip"
type: docs
weight: 80
url: /id/net/aspose.zip.lzip/lziparchive/setsource/
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
using (var archive = new LzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz");

```

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo yang akan dibuka sebagai aliran masukan. |

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz");
}
```

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan dikompres. |

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
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |

## Contoh

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz");
}
```

### Lihat Juga

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


