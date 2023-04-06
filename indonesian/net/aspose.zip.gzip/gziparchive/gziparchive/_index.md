---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: GzipArchive konstruktor. Menginisialisasi instance baru dariGzipArchive kelas disiapkan untuk mengompresi.
type: docs
weight: 10
url: /id/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Menginisialisasi instance baru dari[`GzipArchive`](../) kelas disiapkan untuk mengompresi.

```csharp
public GzipArchive()
```

### Contoh

Contoh berikut menunjukkan cara mengompres file.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Menginisialisasi instance baru dari[`GzipArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| parseHeader | Boolean | Apakah akan mengurai header aliran untuk mencari tahu properti, termasuk nama. Masuk akal hanya untuk aliran yang dapat dicari. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Open`](../open/) metode dekompresi.

### Contoh

Buka arsip dari aliran dan ekstrak ke a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Menginisialisasi instance baru dari[`GzipArchive`](../) kelas.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file arsip. |
| parseHeader | Boolean | Apakah akan mengurai header aliran untuk mencari tahu properti, termasuk nama. Masuk akal hanya untuk aliran yang dapat dicari. |

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

Konstruktor ini tidak melakukan dekompresi. Melihat[`Open`](../open/) metode dekompresi.

### Contoh

Buka arsip dari file dengan jalur dan ekstrak ke a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)


