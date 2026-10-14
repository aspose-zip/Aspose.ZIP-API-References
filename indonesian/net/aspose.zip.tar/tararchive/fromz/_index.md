---
title: "TarArchive.FromZ"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Mengekstrak arsip format Z yang diberikan dan menyusun TarArchive dari data yang diekstrak"
type: docs
weight: 70
url: /id/net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

Mengekstrak arsip format Z yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip Z sepenuhnya diekstrak dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromZ(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Nilai Kembalian

Sebuah instance dari [`TarArchive`](../)

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* bernilai null. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZ(string) {#fromz_1}

Mengekstrak arsip format Z yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip Z sepenuhnya diekstrak dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromZ(string path)
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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


