---
title: "Bzip2Archive.Bzip2Archive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor Bzip2Archive. Menginisialisasi sebuah instance baru dari kelas Bzip2Archive yang disiapkan untuk kompresi."
type: docs
weight: 10
url: /id/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`Bzip2Archive`](../) yang disiapkan untuk kompresi.

```csharp
public Bzip2Archive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Lihat Juga

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream, Bzip2LoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`Bzip2Archive`](../) yang disiapkan untuk dekompresi.

```csharp
public Bzip2Archive(Stream sourceStream, Bzip2LoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | Bzip2LoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Akhir aliran terlalu dini. |
| InvalidDataException | Byte tanda tangan salah. |
| IOException | Terjadi kesalahan I/O. |
| ArgumentNullException | *sourceStream* bernilai null. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(string, Bzip2LoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`Bzip2Archive`](../) yang disiapkan untuk dekompresi.

```csharp
public Bzip2Archive(string path, Bzip2LoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | Bzip2LoadOptions | Opsi untuk memuat arsip. |

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
| EndOfStreamException | Akhir aliran terlalu dini. |
| InvalidDataException | Byte tanda tangan salah. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


