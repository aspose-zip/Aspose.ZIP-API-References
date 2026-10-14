---
title: "LzmaArchive.LzmaArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LzmaArchive. Menginisialisasi instance baru dari kelas LzmaArchive dan menyusun arsip dalam format lzma"
type: docs
weight: 10
url: /id/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Menginisialisasi instance baru dari kelas [`LzmaArchive`](../) dan menyusun arsip dalam format lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengaturan | LzmaArchiveSettings | Sekumpulan pengaturan untuk arsip lzma tertentu. |

### Lihat Juga

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LzmaArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public LzmaArchive(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *source* bernilai null. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Menginisialisasi instance baru dari kelas [`LzmaArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public LzmaArchive(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke sumber arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

## Contoh

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
}
```

### Lihat Juga

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


