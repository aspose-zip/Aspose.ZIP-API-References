---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Mengekstrak arsip LZ4 yang diberikan dan menyusun TarArchive dari data yang diekstrak"
type: docs
weight: 30
url: /id/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Mengekstrak arsip LZ4 yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip LZ4 sepenuhnya diekstrak dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | File di *path* memiliki format yang tidak valid. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| EndOfStreamException | Berkas terlalu pendek. |
| InvalidDataException | File memiliki tanda tangan yang salah. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| InvalidOperationException | Arsip telah dipersiapkan untuk komposisi. |

## Catatan

Aliran ekstraksi LZ4 tidak dapat diposisikan kembali karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat diposisikan kembali di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Mengekstrak arsip LZ4 yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip LZ4 sepenuhnya diekstrak dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Nilai Kembalian

Sebuah instance dari [`TarArchive`](../)

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | Tidak dapat membaca dari *source* |
| ArgumentNullException | *source* bernilai null. |
| EndOfStreamException | *source* terlalu pendek. |
| InvalidDataException | *source* memiliki tanda tangan yang salah. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Aliran ekstraksi LZ4 tidak dapat diposisikan kembali karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat diposisikan kembali di balik layar.

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


