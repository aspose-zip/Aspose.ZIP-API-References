---
title: "GzipArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode GzipArchive. Mengekstrak konten arsip ke direktori yang disediakan"
type: docs
weight: 60
url: /id/net/aspose.zip.gzip/gziparchive/extracttodirectory/
---
## GzipArchive.ExtractToDirectory method

Mengekstrak konten arsip ke direktori yang diberikan.

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
| NotSupportedException | Jika direktori tidak ada, jalur mengandung karakter titik dua (:) yang bukan bagian dari label drive ("C:\"). |
| ArgumentException | *destinationDirectory* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid. Anda dapat menanyakan karakter tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -atau- jalur diawali dengan, atau hanya berisi, karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh jalur adalah sebuah file. -atau- Nama jaringan tidak dikenal. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Jika direktori tidak ada, maka akan dibuat.

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


