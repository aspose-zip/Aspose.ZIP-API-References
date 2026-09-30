---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LzxArchive. Menginisialisasi instance baru dari kelas LzxArchive dan menyusun daftar entri yang dapat diekstrak dari arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Menginisialisasi instance baru dari kelas [`LzxArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | Stream | Sumber arsip. |
| loadOptions | LzxLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *extractionSource* bernilai null. |
| ArgumentException | *extractionSource* tidak mendukung pencarian. |
| InvalidDataException | Tanda tangan arsip salah. - atau - File bukan arsip LZX. |
| NotImplementedException | Arsip Lzx berisi entri yang digabungkan. |
| EndOfStreamException | Aliran *extractionSource* terlalu pendek. |
| ObjectDisposedException | Dilemparkan jika aliran telah ditutup. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Extract`](../../lzxarchiveentry/extract/) untuk dekompresi.

### Lihat Juga

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LzxArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| loadOptions | LzxLoadOptions | Opsi untuk memuat arsip yang ada. |

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
| InvalidDataException | File tersebut rusak. |
| NotImplementedException | Arsip Lzx berisi entri yang digabungkan. |
| EndOfStreamException | Berkas terlalu pendek. |
| ObjectDisposedException | Dilemparkan jika aliran telah ditutup. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Extract`](../../lzxarchiveentry/extract/) untuk dekompresi.

## Contoh

Contoh berikut mengekstrak sebuah arsip, lalu mendekompresi entri pertama ke `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Lihat Juga

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


