---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzipArchive konstruktor. Menginisialisasi instance baru dariLzipArchive .
type: docs
weight: 10
url: /id/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Menginisialisasi instance baru dari[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| settings | LzipArchiveSettings | Pengaturan arsip lzip tertentu dengan definisi ukuran kamus. |

### Lihat juga

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`LzipArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public LzipArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| ArgumentNullException | *sourceStream* adalah nol. |
| InvalidDataException | Header tidak cocok dengan jenis arsip lzip. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`LzipArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public LzipArchive(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |
| InvalidDataException | Header tidak cocok dengan jenis arsip lzip. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Contoh

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Lihat juga

* class [LzipArchive](../)
* ruang nama [Aspose.Zip.Lzip](../../lziparchive/)
* perakitan [Aspose.Zip](../../../)


