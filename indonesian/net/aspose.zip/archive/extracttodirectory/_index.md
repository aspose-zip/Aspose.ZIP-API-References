---
title: "Archive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Archive. Mengekstrak semua file dalam arsip ke direktori yang diberikan"
type: docs
weight: 90
url: /id/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

Mengekstrak semua file dalam arsip ke direktori yang disediakan.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat menempatkan file yang diekstrak. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationDirectory* bernilai null. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter dan nama file harus kurang dari 260 karakter. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, jalur berisi karakter titik dua (:) yang bukan bagian dari label drive (\"C:\\"). |
| ArgumentException | *destinationDirectory* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid. Anda dapat menanyakan karakter tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -atau- jalur diawali dengan, atau hanya berisi, karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh jalur adalah sebuah file. -atau- Nama jaringan tidak dikenal. |
| InvalidDataException | Kata sandi yang diberikan salah. - atau - Arsip rusak. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| EndOfStreamException | Stream tidak berisi cukup byte untuk membaca data yang diminta. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

## Contoh

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


