---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor IsoArchive. Menginisialisasi instance baru dari kelas IsoArchive dan membuat arsip ISO kosong untuk menambahkan file dan direktori baru."
type: docs
weight: 10
url: /id/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Menginisialisasi instance baru dari kelas [`IsoArchive`](../) dan membuat arsip ISO kosong untuk menambahkan file dan direktori baru.

```csharp
public IsoArchive()
```

## Contoh

Contoh berikut menunjukkan cara membuat arsip ISO kosong baru dan menambahkan file ke dalamnya:

```csharp
// Buat arsip ISO kosong baru
using(IsoArchive isoArchive = new IsoArchive())
{
    // Tambahkan file ke arsip ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Simpan arsip ISO ke sebuah file
    isoArchive.Save("new_archive.iso");
}
```

### Lihat Juga

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`IsoArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Harus dapat di-seek. |
| loadOptions | IsoLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan arsip ISO yang valid. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai secara tak terduga. |
| IOException | Terjadi kesalahan I/O. |
| NotSupportedException | Aliran tidak mendukung pembacaan. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`IsoArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |
| loadOptions | IsoLoadOptions | Opsi untuk memuat arsip. |

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
| EndOfStreamException | Berkas terlalu pendek. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


