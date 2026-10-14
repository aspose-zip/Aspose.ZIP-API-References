---
title: "LzipArchive.LzipArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LzipArchive. Menginisialisasi instance baru dari LzipArchive"
type: docs
weight: 10
url: /id/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Menginisialisasi instance baru dari [`LzipArchive`](../).

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengaturan | LzipArchiveSettings | Pengaturan arsip lzip tertentu dengan definisi ukuran kamus. |

### Lihat Juga

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(Stream, LzipLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LzipArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public LzipArchive(Stream sourceStream, LzipLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| opsi | LzipLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| ArgumentNullException | *sourceStream* bernilai null. |
| InvalidDataException | Header tidak cocok dengan tipe arsip lzip. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(string, LzipLoadOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`LzipArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public LzipArchive(string path, LzipLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke sumber arsip. |
| opsi | LzipLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| InvalidDataException | Header tidak cocok dengan tipe arsip lzip. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

## Contoh

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Lihat Juga

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


