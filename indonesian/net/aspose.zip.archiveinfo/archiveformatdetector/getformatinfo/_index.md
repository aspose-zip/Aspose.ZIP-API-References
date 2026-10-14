---
title: "GetFormatInfo"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: 
type: docs
weight: 20
url: /id/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Mendapatkan info format.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip. |

### Nilai Kembalian

Informasi tentang format arsip atau null jika format tidak terdeteksi.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *fileName* adalah null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Nama file *fileName* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *fileName* ditolak. |
| PathTooLongException | Nama file *fileName* yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File pada *fileName* berisi titik dua (:) di tengah string. |
| IOException | Terjadi kesalahan I/O saat membuka file. |

### Lihat Juga

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Mendapatkan info format.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran file arsip. |

### Nilai Kembalian

Informasi tentang format arsip atau null jika format tidak terdeteksi.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *stream* bernilai null. |
| ArgumentException | *stream* tidak dapat di-seek. |

### Lihat Juga

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- JANGAN SUNTING: dihasilkan oleh xmldocmd untuk Aspose.Zip.dll -->
