---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor ArjArchive. Menginisialisasi sebuah instance baru dari kelas ArjArchive dan menyusun daftar entri yang dapat diekstrak dari arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`ArjArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | Stream | Sumber arsip. |
| loadOptions | ArjLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *extractionSource* bernilai null. |
| ArgumentException | &gt;*extractionSource* tidak mendukung pencarian. |
| InvalidDataException | Tanda tangan arsip salah. - atau - File bukan arsip ARJ. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum semua byte header atau byte nama dibaca. |
| NotSupportedException | Arsip rusak. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Extract`](../../arjentryplain/extract/) untuk mendekompresi.

### Lihat Juga

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`ArjArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | ArjLoadOptions | Opsi untuk memuat arsip yang ada. |

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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum semua byte header atau byte nama dibaca. |
| InvalidDataException | Nomor ajaib ARJ tidak valid atau ukuran header berada di luar jangkauan. |

## Catatan

Konstruktor ini tidak membuka paket entri apa pun. Lihat metode [`Extract`](../../arjentryplain/extract/) untuk mendekompresi.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


