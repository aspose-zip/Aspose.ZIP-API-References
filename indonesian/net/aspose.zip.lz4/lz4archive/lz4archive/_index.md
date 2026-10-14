---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor Lz4Archive. Menginisialisasi sebuah instance baru dari kelas Lz4Archive yang disiapkan untuk dekompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`Lz4Archive`](../) yang disiapkan untuk dekompresi.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | Lz4LoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | Tidak dapat membaca dari *sourceStream* |
| ArgumentNullException | *sourceStream* bernilai null. |
| EndOfStreamException | *sourceStream* terlalu pendek. |
| InvalidDataException | *sourceStream* memiliki tanda tangan yang salah. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | Lz4LoadOptions | Opsi untuk memuat arsip. |

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
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`Lz4Archive`](../) yang disiapkan untuk kompresi.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengaturan | Lz4ArchiveSetting | Pengaturan dari arsip yang disusun. |

### Lihat Juga

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


