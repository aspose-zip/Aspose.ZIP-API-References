---
title: TarArchive.TarArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive konstruktor. Menginisialisasi instance baru dariTarArchive kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Menginisialisasi instance baru dari[`TarArchive`](../) kelas.

```csharp
public TarArchive()
```

### Contoh

Contoh berikut menunjukkan cara mengompres file.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`Archive`](../../../aspose.zip/archive/) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public TarArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Itu harus dicari. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidDataException | *sourceStream* tidak dapat dicari. |

### Perkataan

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../tarentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`TarArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public TarArchive(string path)
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

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../tarentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


