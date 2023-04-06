---
title: Archive.ExtractToDirectory
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Ekstrak semua file dalam arsip ke direktori yang disediakan.
type: docs
weight: 80
url: /id/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

Ekstrak semua file dalam arsip ke direktori yang disediakan.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori untuk menempatkan file yang diekstraksi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *destinationDirectory* adalah nol. |
| PathTooLongException | Jalur yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter dan nama file harus kurang dari 260 karakter. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, path berisi karakter titik dua (:) yang bukan merupakan bagian dari label drive ("C:\"). |
| ArgumentException | *destinationDirectory*adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau beberapa karakter yang tidak valid. Anda dapat meminta karakter yang tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -or- path diawali dengan, atau berisi, hanya karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh path adalah file. -atau- Nama jaringan tidak diketahui. |
| InvalidDataException | Kata sandi yang salah telah diberikan. |

### Perkataan

Jika direktori tidak ada, itu akan dibuat.

### Contoh

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


