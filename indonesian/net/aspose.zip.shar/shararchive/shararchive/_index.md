---
title: "SharArchive.SharArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SharArchive. Menginisialisasi instance baru dari kelas SharArchive"
type: docs
weight: 10
url: /id/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Menginisialisasi instance baru dari kelas [`SharArchive`](../).

```csharp
public SharArchive()
```

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah file.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

Menginisialisasi instance baru dari kelas [`SharArchive`](../) yang dipersiapkan untuk dekompresi.

```csharp
public SharArchive(string path)
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

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


