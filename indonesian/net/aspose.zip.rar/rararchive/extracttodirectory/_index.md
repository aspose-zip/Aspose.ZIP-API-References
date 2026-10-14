---
title: "RarArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode RarArchive. Mengekstrak semua file dalam arsip ke direktori yang diberikan"
type: docs
weight: 40
url: /id/net/aspose.zip.rar/rararchive/extracttodirectory/
---
## RarArchive.ExtractToDirectory method

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
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

Untuk mengekstrak `RarArchive` yang terenkripsi gunakan [`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/)

## Contoh

```csharp
using (var archive = new RarArchive("archive.rar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat Juga

* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


