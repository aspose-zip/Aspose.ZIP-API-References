---
title: "Archive.Archive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Archive constructor. Menginisialisasi instance baru dari kelas Archive dengan pengaturan opsional untuk entri-entrinya"
type: docs
weight: 10
url: /id/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Menginisialisasi instance baru dari kelas [`Archive`](../) dengan pengaturan opsional untuk entri-entrinya.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang baru ditambahkan. Jika tidak ditentukan, kompresi Deflate yang paling umum tanpa enkripsi akan digunakan. |

## Contoh

Contoh berikut menunjukkan cara mengompres satu file dengan pengaturan default.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Lihat Juga

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Menginisialisasi instance baru dari kelas [`Archive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | ArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang baru ditambahkan. Jika tidak ditentukan, kompresi Deflate yang paling umum tanpa enkripsi akan digunakan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindai, ketika dimuat tanpa mengatur [`ForwardOnly`](../../archiveloadoptions/forwardonly/). |
| InvalidDataException | Header enkripsi untuk AES bertentangan dengan metode kompresi WinZip. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| NotSupportedException | Dilempar ketika arsip dimuat dari aliran hanya-baca dalam mode evaluasi. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Open`](../../archiveentry/open/) untuk mendekompresi.

## Contoh

Contoh berikut mengekstrak arsip yang terenkripsi, lalu mendekompresi entri pertama ke `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Lihat Juga

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Menginisialisasi instance baru dari kelas [`Archive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| loadOptions | ArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../../archiveentry/) yang baru ditambahkan. Jika tidak ditentukan, kompresi Deflate yang paling umum tanpa enkripsi akan digunakan. |

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
| InvalidDataException | File tersebut rusak. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Open`](../../archiveentry/open/) untuk mendekompresi.

## Contoh

Contoh berikut mengekstrak arsip yang terenkripsi, lalu mendekompresi entri pertama ke `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Lihat Juga

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, string[], ArchiveLoadOptions) {#constructor_3}

Menginisialisasi instance baru dari kelas [`Archive`](../) dari arsip ZIP multi-volume dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public Archive(string mainSegment, string[] segmentsInOrder, ArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mainSegment | String | Jalur ke segmen terakhir arsip multi-volume dengan direktori pusat. |
| segmentsInOrder | String[] | Jalur ke setiap segmen kecuali yang terakhir dari arsip zip multi-volume dengan memperhatikan urutan. |
| loadOptions | ArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Tidak dapat memuat header ZIP karena file yang disediakan rusak. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| FileNotFoundException | File yang ditentukan dalam jalur tidak ditemukan. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Jalur yang ditentukan adalah sebuah direktori. -atau- Pemanggil tidak memiliki izin yang diperlukan. |

## Contoh

Contoh ini mengekstrak ke sebuah direktori arsip yang terdiri dari tiga segmen.

```csharp
using (Archive a = new Archive("archive.zip", new string[] { "archive.z01", "archive.z02" }))
{
    a.ExtractToDirectory("destination");
}
```

### Lihat Juga

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


