---
title: XarArchive.XarArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: XarArchive konstruktor. Menginisialisasi instance baru dariXarArchive kelas dan menulis daftar entri dapat diekstraksi dari arsip.
type: docs
weight: 10
url: /id/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Menginisialisasi instance baru dari[`XarArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public XarArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Itu harus dicari. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* adalah nol. |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | *sourceStream* bukan arsip xar yang valid. |

### Perkataan

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../xarfileentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [XarArchive](../)
* ruang nama [Aspose.Zip.Xar](../../xararchive/)
* perakitan [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Menginisialisasi instance baru dari[`XarArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public XarArchive(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file arsip. |

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

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../xarfileentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [XarArchive](../)
* ruang nama [Aspose.Zip.Xar](../../xararchive/)
* perakitan [Aspose.Zip](../../../)


