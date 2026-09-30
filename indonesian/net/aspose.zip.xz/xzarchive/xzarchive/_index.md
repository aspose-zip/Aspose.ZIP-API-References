---
title: "XzArchive.XzArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor XzArchive. Menginisialisasi instance baru dari kelas XzArchive dan menyusun arsip dalam format xz"
type: docs
weight: 10
url: /id/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Menginisialisasi instance baru dari kelas [`XzArchive`](../) dan menyusun arsip dalam format xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengaturan | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, tipe pemeriksaan. |

### Lihat Juga

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(Stream, XzLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`XzArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public XzArchive(Stream source, XzLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |
| opsi | XzLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* bernilai null. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |
| InvalidDataException | Data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(string, XzLoadOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`XzArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public XzArchive(string path, XzLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke sumber arsip. |
| opsi | XzLoadOptions | Opsi untuk memuat arsip. |

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
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


