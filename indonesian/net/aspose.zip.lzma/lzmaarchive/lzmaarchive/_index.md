---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzmaArchive konstruktor. Menginisialisasi instance baru dariLzmaArchive kelas dan menyusun arsip dalam format lzma.
type: docs
weight: 10
url: /id/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Menginisialisasi instance baru dari[`LzmaArchive`](../) kelas dan menyusun arsip dalam format lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Set pengaturan arsip lzma tertentu. |

### Lihat juga

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`LzmaArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public LzmaArchive(Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* adalah nol. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Lihat juga

* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`LzmaArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public LzmaArchive(string path)
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

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Contoh

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Lihat juga

* class [LzmaArchive](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchive/)
* perakitan [Aspose.Zip](../../../)


