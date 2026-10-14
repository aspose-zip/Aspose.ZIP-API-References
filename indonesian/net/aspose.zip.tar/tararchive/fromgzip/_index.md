---
title: "TarArchive.FromGZip"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Mengekstrak arsip gzip yang disediakan dan menyusun TarArchive dari data yang diekstrak"
type: docs
weight: 20
url: /id/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Mengekstrak arsip gzip yang disediakan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: arsip gzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromGZip(Stream source)
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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Aliran ekstraksi GZip tidak dapat dicari (seekable) karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Mengekstrak arsip gzip yang disediakan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: arsip gzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromGZip(string path)
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
| IOException | Terjadi kesalahan I/O saat membuka file. |

## Catatan

Aliran ekstraksi GZip tidak dapat dicari (seekable) karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


