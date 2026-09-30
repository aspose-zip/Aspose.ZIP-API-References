---
title: "SevenZipArchive.SevenZipArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SevenZipArchive. Menginisialisasi sebuah instansi baru dari kelas SevenZipArchive dengan pengaturan opsional untuk entri‑nya"
type: docs
weight: 10
url: /id/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Menginisialisasi sebuah instansi baru dari kelas [`SevenZipArchive`](../) dengan pengaturan opsional untuk entri‑nya.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) yang baru ditambahkan. Jika tidak ditentukan, kompresi LZMA tanpa enkripsi akan digunakan. |

## Contoh

Contoh berikut menunjukkan cara mengompresi satu file dengan pengaturan default: kompresi LZMA tanpa enkripsi.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Lihat Juga

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, string) {#constructor_2}

Menginisialisasi sebuah instansi baru dari kelas [`SevenZipArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public SevenZipArchive(Stream sourceStream, string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| password | String | Kata sandi opsional untuk dekripsi. Jika nama file dienkripsi, kata sandi harus ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| ArgumentNullException | *sourceStream* bernilai null. |
| NotImplementedException | Arsip berisi lebih dari satu pengode. Sekarang hanya kompresi LZMA yang didukung. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) untuk dekompresi.

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, string) {#constructor_4}

Menginisialisasi sebuah instansi baru dari kelas [`SevenZipArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public SevenZipArchive(string path, string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| password | String | Kata sandi opsional untuk dekripsi. Jika nama file dienkripsi, kata sandi harus ada. |

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

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) untuk dekompresi.

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, SevenZipLoadOptions) {#constructor_1}

Menginisialisasi sebuah instansi baru dari kelas [`SevenZipArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public SevenZipArchive(Stream sourceStream, SevenZipLoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| opsi | SevenZipLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| ArgumentNullException | *sourceStream* bernilai null. |
| NotImplementedException | Arsip berisi lebih dari satu pengode. Sekarang hanya kompresi LZMA yang didukung. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) untuk dekompresi.

## Contoh

Ekstrak arsip yang dienkripsi. Izinkan hingga 60 detik untuk melanjutkan, batalkan setelah periode tersebut.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### Lihat Juga

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, SevenZipLoadOptions) {#constructor_3}

Menginisialisasi sebuah instansi baru dari kelas [`SevenZipArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public SevenZipArchive(string path, SevenZipLoadOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| opsi | SevenZipLoadOptions | Opsi untuk memuat arsip yang ada. |

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

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) untuk dekompresi.

## Contoh

Ekstrak arsip yang dienkripsi. Izinkan hingga 60 detik untuk melanjutkan, batalkan setelah periode tersebut.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### Lihat Juga

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string[], string) {#constructor_5}

Menginisialisasi instance baru dari kelas [`SevenZipArchive`](../) dari arsip 7z multi-volume dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public SevenZipArchive(string[] parts, string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| parts | String[] | Jalur ke setiap segmen arsip 7z multi-volume dengan memperhatikan urutan |
| password | String | Kata sandi opsional untuk dekripsi. Jika nama file dienkripsi, kata sandi harus ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *parts* bernilai null. |
| ArgumentException | *parts* tidak memiliki entri. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Jalur ke file kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file ditolak. |
| PathTooLongException | Jalur yang ditentukan ke bagian, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File pada jalur mengandung titik dua (:) di tengah string. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new string[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" }))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


