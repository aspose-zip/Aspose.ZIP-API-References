---
title: "WimImage.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode WimImage. Mengekstrak semua file dalam gambar ke direktori yang diberikan"
type: docs
weight: 40
url: /id/net/aspose.zip.wim/wimimage/extracttodirectory/
---
## WimImage.ExtractToDirectory method

Mengekstrak semua file dalam gambar ke direktori yang diberikan.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat menempatkan file yang diekstrak. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | jalur bernilai null |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter dan nama file harus kurang dari 260 karakter. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, jalur berisi karakter titik dua (:) yang bukan bagian dari label drive (\"C:\\"). |
| ArgumentException | jalur adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid. Anda dapat memeriksa karakter tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -atau- jalur diawali dengan, atau hanya berisi, karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh jalur adalah sebuah file. -atau- Nama jaringan tidak dikenal. |
| InvalidDataException | Arsip rusak. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

## Contoh

```csharp
using (var archive = new WimArchive("install.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [WimImage](../)
* namespace [Aspose.Zip.Wim](../../wimimage/)
* assembly [Aspose.Zip](../../../)


