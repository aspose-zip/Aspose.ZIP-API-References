---
title: "GzipArchive.GzipArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor GzipArchive. Menginisialisasi sebuah instance baru dari kelas GzipArchive yang disiapkan untuk kompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`GzipArchive`](../) yang disiapkan untuk kompresi.

```csharp
public GzipArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`GzipArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| parseHeader | Boolean | Apakah akan mengurai header aliran untuk menentukan properti, termasuk nama. Hanya masuk akal untuk aliran yang dapat dicari. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| EndOfStreamException | *sourceStream* terlalu pendek. |
| InvalidDataException | *sourceStream* memiliki tanda tangan yang salah. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, GzipLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`GzipArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public GzipArchive(Stream sourceStream, GzipLoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| opsi | GzipLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| EndOfStreamException | *sourceStream* terlalu pendek. |
| InvalidDataException | *sourceStream* memiliki tanda tangan yang salah. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz"), options))
  archive.Extract(ms);
```

### Lihat Juga

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, GzipLoadOptions) {#constructor_3}

Menginisialisasi sebuah instance baru dari kelas [`GzipArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public GzipArchive(string path, GzipLoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| opsi | GzipLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| EndOfStreamException | Berkas terlalu pendek. |
| InvalidDataException | Data dalam file memiliki tanda tangan yang salah. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive("archive.gz", options))
  archive.Extract(ms);
```

### Lihat Juga

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_4}

Menginisialisasi sebuah instance baru dari kelas [`GzipArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| parseHeader | Boolean | Apakah akan mengurai header aliran untuk menentukan properti, termasuk nama. Hanya masuk akal untuk aliran yang dapat dicari. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| EndOfStreamException | Berkas terlalu pendek. |
| InvalidDataException | Data dalam file memiliki tanda tangan yang salah. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


