---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "ZstandardArchive konstruktor. Menginisialisasi instance baru dari kelas ZstandardArchive yang dipersiapkan untuk kompresi."
type: docs
weight: 10
url: /id/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Menginisialisasi instance baru dari kelas [`ZstandardArchive`](../) yang dipersiapkan untuk kompresi.

```csharp
public ZstandardArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Lihat Juga

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`ZstandardArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| opsi | ZstandardLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai secara tak terduga. |
| IOException | Terjadi kesalahan I/O. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| opsi | ZstandardLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai secara tak terduga. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


