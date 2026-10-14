---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LhaArchive. Menginisialisasi instance baru dari kelas LhaArchive dan menyusun daftar entri yang dapat diekstrak dari arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Menginisialisasi instance baru dari kelas [`LhaArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | LhaLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | Data tidak sesuai ditemukan. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan ketika objek telah dibuang. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Extract`](../../lhaarchiveentry/extract/) untuk mendekompresi.

### Lihat Juga

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LhaArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| loadOptions | LhaLoadOptions | Opsi untuk memuat arsip yang ada. |

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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan ketika objek telah dibuang. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Extract`](../../lhaarchiveentry/extract/) untuk mendekompresi.

## Contoh

Contoh berikut mengekstrak sebuah arsip, lalu mendekompresi entri pertama ke `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Lihat Juga

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


