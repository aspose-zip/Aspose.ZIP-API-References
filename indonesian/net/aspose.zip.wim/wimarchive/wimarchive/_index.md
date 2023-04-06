---
title: WimArchive.WimArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: WimArchive konstruktor. Menginisialisasi instance baru dariWimArchive kelas dan menulis daftar entri dapat diekstraksi dari arsip.
type: docs
weight: 10
url: /id/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream) {#constructor}

Menginisialisasi instance baru dari[`WimArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public WimArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. Itu harus dicari. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* adalah nol. |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | *sourceStream* bukan arsip wim yang valid. |

### Perkataan

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../wimfileentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [WimArchive](../)
* ruang nama [Aspose.Zip.Wim](../../wimarchive/)
* perakitan [Aspose.Zip](../../../)

---

## WimArchive(string) {#constructor_1}

Menginisialisasi instance baru dari[`WimArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public WimArchive(string path)
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

Konstruktor ini tidak membongkar entri apa pun. Melihat[`Open`](../../wimfileentry/open/)metode unpacking.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke direktori.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [WimArchive](../)
* ruang nama [Aspose.Zip.Wim](../../wimarchive/)
* perakitan [Aspose.Zip](../../../)


