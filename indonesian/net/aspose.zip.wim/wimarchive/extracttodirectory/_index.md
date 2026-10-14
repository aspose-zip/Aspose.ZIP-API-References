---
title: "WimArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode WimArchive. Mengekstrak arsip ke file berdasarkan jalur"
type: docs
weight: 90
url: /id/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Mengekstrak arsip ke file berdasarkan jalur.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat menempatkan file yang diekstrak. |

### Nilai Kembalian

Info tentang file yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *destinationDirectory* bernilai null |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter dan nama file harus kurang dari 260 karakter. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, jalur berisi karakter titik dua (:) yang bukan bagian dari label drive ("C:\") - atau - arsip WIM bersifat multi-bagian. |
| ArgumentException | jalur adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid. Anda dapat memeriksa karakter tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -atau- jalur diawali dengan, atau hanya berisi, karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh jalur adalah sebuah file. -atau- Nama jaringan tidak dikenal. |
| InvalidDataException | Arsip rusak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

### Lihat Juga

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


