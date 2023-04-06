---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2Archive konstruktor. Menginisialisasi instance baru dariBzip2Archive kelas disiapkan untuk mengompresi.
type: docs
weight: 10
url: /id/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Menginisialisasi instance baru dari[`Bzip2Archive`](../) kelas disiapkan untuk mengompresi.

```csharp
public Bzip2Archive()
```

### Contoh

Contoh berikut menunjukkan cara mengompres file.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`Bzip2Archive`](../) kelas disiapkan untuk dekompresi.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Open`](../open/) metode dekompresi.

### Contoh

Buka arsip dari aliran dan ekstrak ke a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Menginisialisasi instance baru dari[`Bzip2Archive`](../) kelas disiapkan untuk dekompresi.

```csharp
public Bzip2Archive(string path)
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

Konstruktor ini tidak melakukan dekompresi. Melihat[`Open`](../open/) metode dekompresi.

### Contoh

Buka arsip dari file dengan jalur dan ekstrak ke a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)


