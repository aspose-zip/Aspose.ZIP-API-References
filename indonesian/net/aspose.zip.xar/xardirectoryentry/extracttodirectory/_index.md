---
title: "XarDirectoryEntry.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode XarDirectoryEntry. Mengekstrak semua file dalam direktori saat ini ke direktori yang diberikan"
type: docs
weight: 50
url: /id/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Mengekstrak semua file di direktori saat ini ke direktori yang diberikan.

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
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

## Contoh

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   ((XarDirectoryEntry)archive.Entries[0]).ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [XarDirectoryEntry](../)
* namespace [Aspose.Zip.Xar](../../xardirectoryentry/)
* assembly [Aspose.Zip](../../../)


