---
title: "RarArchive.RarArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor RarArchive. Menginisialisasi sebuah instance baru dari kelas RarArchive dan menyusun daftar entri yang dapat diekstrak dari arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`RarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| loadOptions | RarArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

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
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Open`](../../rararchiveentry/open/) untuk mendekompresi.

## Contoh

Contoh berikut mengekstrak sebuah arsip, lalu mendekompresi entri pertama ke `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`RarArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | RarArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | Tanda tangan arsip salah. - atau - File bukan arsip RAR. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`Open`](../../rararchiveentry/open/) untuk mendekompresi.

## Contoh

Contoh berikut mendekripsi dan mendekompresi entri pertama ke `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


