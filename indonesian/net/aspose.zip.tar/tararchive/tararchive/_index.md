---
title: "TarArchive.TarArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor TarArchive. Menginisialisasi sebuah instance baru dari kelas TarArchive"
type: docs
weight: 10
url: /id/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`TarArchive`](../).

```csharp
public TarArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(Stream, TarLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`TarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public TarArchive(Stream sourceStream, TarLoadOptions loadOptions = null)
```

| Parameter | Deskripsi |
| --- | --- |
| sourceStream | Sumber arsip. Harus dapat di-seek. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| ArgumentNullException | *sourceStream* bernilai null. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../tarentry/open/) untuk melakukan unpacking.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(string, TarLoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`TarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public TarArchive(string path, TarLoadOptions loadOptions = null)
```

| Parameter | Deskripsi |
| --- | --- |
| path | Jalur ke berkas arsip. |

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

## Catatan

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [`Open`](../../tarentry/open/) untuk melakukan unpacking.

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```csharp
using (var archive = new TarArchive("archive.tar", new TarLoadOptions() { CancellationToken = cancellationToken }))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


