---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: CpioArchive konstruktor. Menginisialisasi instance baru dariCpioArchive kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Menginisialisasi instance baru dari[`CpioArchive`](../) kelas.

```csharp
public CpioArchive()
```

### Contoh

Contoh berikut menunjukkan cara mengompres file.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`CpioArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Itu harus dicari. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* adalah nol. |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | *sourceStream* bukan arsip cpio yang valid. |

### Perkataan

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../cpioentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`CpioArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public CpioArchive(string path)
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

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../cpioentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)


