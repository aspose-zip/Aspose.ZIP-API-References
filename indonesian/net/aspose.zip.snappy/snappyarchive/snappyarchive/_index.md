---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: SnappyArchive konstruktor. Menginisialisasi instance baru dariSnappyArchive kelas disiapkan untuk mengompresi.
type: docs
weight: 10
url: /id/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Menginisialisasi instance baru dari[`SnappyArchive`](../) kelas disiapkan untuk mengompresi.

```csharp
public SnappyArchive()
```

### Contoh

Contoh berikut menunjukkan cara mengompres file.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Lihat juga

* class [SnappyArchive](../)
* ruang nama [Aspose.Zip.Snappy](../../snappyarchive/)
* perakitan [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`SnappyArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* ruang nama [Aspose.Zip.Snappy](../../snappyarchive/)
* perakitan [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`SnappyArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Lihat juga

* class [SnappyArchive](../)
* ruang nama [Aspose.Zip.Snappy](../../snappyarchive/)
* perakitan [Aspose.Zip](../../../)


