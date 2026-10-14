---
title: "CabArchive.CabArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor CabArchive. Menginisialisasi sebuah instance baru dari kelas CabArchive yang disiapkan untuk kompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(CabEntrySettings) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`CabArchive`](../) yang disiapkan untuk kompresi.

```csharp
public CabArchive(CabEntrySettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | CabEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`CabEntry`](../../cabentry/) yang baru ditambahkan. Jika tidak ditentukan, kompresi MSZIP akan digunakan. |

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cab");
}
```

Kompres sebuah file menggunakan pengaturan kompresi tertentu.

```csharp
using (var archive = new CabArchive())
{
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("entry.bin", "data.bin", settings);
    archive.Save("archive.cab");
}
```

### Lihat Juga

* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(Stream, CabLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`CabArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public CabArchive(Stream sourceStream, CabLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Harus dapat di-seek. |
| loadOptions | CabLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan arsip CAB yang valid. |
| EndOfStreamException | Aliran terlalu pendek. |
| ObjectDisposedException | Dilemparkan ketika aliran telah dibuang. |
| IOException | Terjadi kesalahan I/O. |
| NotSupportedException | Aliran tidak mendukung pencarian, misalnya jika aliran dibangun dari pipa atau output konsol. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../cabentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(string, CabLoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`CabArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public CabArchive(string path, CabLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | CabLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| EndOfStreamException | Berkas terlalu pendek. |
| InvalidDataException | Nomor ajaib CAB tidak valid atau ukuran header tidak cocok. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../cabentry/open/) untuk mengekstrak.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new CabArchive("archive.cab")) hj
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


