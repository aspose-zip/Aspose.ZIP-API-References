---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveInstanceInfo metode. Mendapat info format arsip.
type: docs
weight: 50
url: /id/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Mendapat info format arsip.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama file dari file arsip. |

### Nilai Pengembalian

Informasi tentang format arsip atau null jika format tidak terdeteksi.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *fileName* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*fileName* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*fileName* ditolak. |
| PathTooLongException | Yang ditentukan*fileName* melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*fileName* berisi titik dua (:) di tengah string. |
| IOException | Terjadi kesalahan I/O saat membuka file. |

### Lihat juga

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* ruang nama [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* perakitan [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Mendapat info format arsip.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Aliran file arsip. |

### Nilai Pengembalian

Informasi tentang format arsip atau null jika format tidak terdeteksi.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *stream* adalah nol. |
| ArgumentException | *stream* tidak dapat dicari. |

### Lihat juga

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* ruang nama [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* perakitan [Aspose.Zip](../../../)


