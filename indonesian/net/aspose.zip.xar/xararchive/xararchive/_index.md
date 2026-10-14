---
title: "XarArchive.XarArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor XarArchive. Menginisialisasi sebuah instance baru dari kelas XarArchive."
type: docs
weight: 10
url: /id/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(XarCompressionSettings) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`XarArchive`](../).

```csharp
public XarArchive(XarCompressionSettings defaultCompressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultCompressionSettings | XarCompressionSettings | Pengaturan kompresi default, diterapkan pada semua entri dalam arsip. |

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Lihat Juga

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(Stream, XarLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`XarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public XarArchive(Stream sourceStream, XarLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Harus dapat di-seek. |
| loadOptions | XarLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan arsip xar yang valid. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../xarfileentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(string, XarLoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`XarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public XarArchive(string path, XarLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | XarLoadOptions | Opsi untuk memuat arsip. |

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
| InvalidDataException | File di *path* bukan arsip xar yang valid. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../xarfileentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


