---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Mengekstrak arsip Zstandard yang diberikan dan menyusun TarArchive dari data yang diekstrak."
type: docs
weight: 80
url: /id/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Mengekstrak arsip Zstandard yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip Zstandard diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Nilai Kembalian

Sebuah instance dari [`TarArchive`](../)

### Pengecualian

| exception | kondisi |
| --- | --- |
| IOException | Aliran Zstandard rusak atau tidak dapat dibaca. |
| InvalidDataException | Data rusak. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Mengekstrak arsip Zstandard yang diberikan dan menyusun [`TarArchive`](../) dari data yang diekstrak.

Penting: Arsip Zstandard diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Aliran Zstandard rusak atau tidak dapat dibaca. |
| InvalidDataException | Data rusak. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


