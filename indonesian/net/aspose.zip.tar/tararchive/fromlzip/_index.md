---
title: "TarArchive.FromLZip"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Mengekstrak arsip lzip yang diberikan dan menyusun TarArchive dari data yang diekstrak."
type: docs
weight: 40
url: /id/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Mengekstrak arsip lzip yang disediakan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: arsip lzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Nilai Kembalian

Sebuah instance dari [`TarArchive`](../)

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidDataException | Arsip rusak. |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* bernilai null. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |

## Catatan

Aliran ekstraksi Lzip tidak dapat dicari (seekable) karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Mengekstrak arsip lzip yang disediakan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: arsip lzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromLZip(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |

### Nilai Kembalian

Sebuah instance dari [`TarArchive`](../)

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | File di *path* memiliki format yang tidak valid. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | Arsip rusak. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| IOException | Terjadi kesalahan I/O. |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |

## Catatan

Aliran ekstraksi Lzip tidak dapat dicari (seekable) karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


