---
title: "CabArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CabArchive. Mengekstrak semua file dalam arsip ke direktori yang disediakan."
type: docs
weight: 60
url: /id/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

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
| ArgumentNullException | jalur bernilai null |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, sebuah path berisi karakter titik dua (:) yang bukan bagian dari label drive ("C:\"). |
| ArgumentException | jalur adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid. Anda dapat memeriksa karakter tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -atau- jalur diawali dengan, atau hanya berisi, karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh jalur adalah sebuah file. -atau- Nama jaringan tidak dikenal. |
| InvalidDataException | Arsip rusak. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip telah disiapkan untuk komposisi dan tidak dapat diekstrak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

## Contoh

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


