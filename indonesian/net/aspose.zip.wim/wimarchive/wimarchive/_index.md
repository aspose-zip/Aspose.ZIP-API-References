---
title: "WimArchive.WimArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor WimArchive. Menginisialisasi instance baru dari kelas WimArchive dan menyusun daftar entri yang dapat diekstrak dari arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream, WimLoadOptions) {#constructor}

Menginisialisasi instance baru dari kelas [`WimArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public WimArchive(Stream sourceStream, WimLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Harus dapat di-seek. |
| loadOptions | WimLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan arsip wim yang valid. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| NotSupportedException | Header menunjukkan arsip multipart. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../wimfileentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)

---

## WimArchive(string, WimLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`WimArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public WimArchive(string path, WimLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | WimLoadOptions | Opsi untuk memuat arsip yang ada. |

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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| InvalidDataException | Header menunjukkan arsip multipart. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../wimfileentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


