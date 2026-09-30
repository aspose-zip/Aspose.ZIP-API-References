---
title: "CpioArchive.CpioArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor CpioArchive. Menginisialisasi instansi baru dari kelas CpioArchive"
type: docs
weight: 10
url: /id/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Menginisialisasi instansi baru dari kelas [`CpioArchive`](../).

```csharp
public CpioArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Menginisialisasi instansi baru dari kelas [`CpioArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Harus dapat di-seek. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan arsip cpio yang valid. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum semua byte header atau byte nama dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../cpioentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Menginisialisasi instansi baru dari kelas [`CpioArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public CpioArchive(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |

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
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum semua byte header atau byte nama dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../cpioentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


