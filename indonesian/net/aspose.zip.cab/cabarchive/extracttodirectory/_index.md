---
title: CabArchive.ExtractToDirectory
second_title: Aspose.ZIP untuk Referensi .NET API
description: CabArchive metode. Ekstrak semua file dalam arsip ke direktori yang disediakan.
type: docs
weight: 40
url: /id/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

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
| ArgumentNullException | jalan adalah nol |
| PathTooLongException | Jalur yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, path berisi karakter titik dua (:) yang bukan merupakan bagian dari label drive ("C:\"). |
| ArgumentException | path adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau beberapa karakter yang tidak valid. Anda dapat meminta karakter yang tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -or- path diawali dengan, atau berisi, hanya karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh path adalah file. -atau- Nama jaringan tidak diketahui. |

### Perkataan

Jika direktori tidak ada, itu akan dibuat.

### Contoh

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Lihat juga

* class [CabArchive](../)
* ruang nama [Aspose.Zip.Cab](../../cabarchive/)
* perakitan [Aspose.Zip](../../../)


