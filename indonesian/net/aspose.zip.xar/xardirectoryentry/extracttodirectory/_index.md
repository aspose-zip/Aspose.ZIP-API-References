---
title: XarDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP untuk Referensi .NET API
description: XarDirectoryEntry metode. Ekstrak semua file di direktori saat ini ke direktori yang disediakan.
type: docs
weight: 50
url: /id/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Ekstrak semua file di direktori saat ini ke direktori yang disediakan.

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
| PathTooLongException | Jalur yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter dan nama file harus kurang dari 260 karakter. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses direktori yang ada. |
| NotSupportedException | Jika direktori tidak ada, path berisi karakter titik dua (:) yang bukan merupakan bagian dari label drive ("C:\"). |
| ArgumentException | path adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau beberapa karakter yang tidak valid. Anda dapat meminta karakter yang tidak valid dengan menggunakan metode System.IO.Path.GetInvalidPathChars. -or- path diawali dengan, atau berisi, hanya karakter titik dua (:). |
| IOException | Direktori yang ditentukan oleh path adalah file. -atau- Nama jaringan tidak diketahui. |

### Perkataan

Jika direktori tidak ada, itu akan dibuat.

### Contoh

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.Directories.First().ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [XarDirectoryEntry](../)
* ruang nama [Aspose.Zip.Xar](../../xardirectoryentry/)
* perakitan [Aspose.Zip](../../../)


