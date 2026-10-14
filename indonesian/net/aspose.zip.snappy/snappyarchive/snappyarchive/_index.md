---
title: "SnappyArchive.SnappyArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SnappyArchive. Menginisialisasi instance baru dari kelas SnappyArchive yang disiapkan untuk kompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Menginisialisasi instance baru dari kelas [`SnappyArchive`](../) yang disiapkan untuk kompresi.

```csharp
public SnappyArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### Lihat Juga

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari kelas [`SnappyArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public SnappyArchive(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* bernilai null. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Menginisialisasi instance baru dari kelas [`SnappyArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public SnappyArchive(string path)
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
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

## Contoh

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Lihat Juga

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


