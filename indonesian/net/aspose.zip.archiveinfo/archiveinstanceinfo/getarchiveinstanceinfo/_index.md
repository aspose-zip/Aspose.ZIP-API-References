---
title: "ArchiveInstanceInfo.GetArchiveInstanceInfo"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArchiveInstanceInfo. Mengembalikan info instance arsip"
type: docs
weight: 10
url: /id/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Mendapatkan info instance arsip.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip. |

### Nilai Kembalian

Informasi tentang instance arsip atau null jika format tidak terdeteksi.

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
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| FileNotFoundException | File yang ditentukan tidak ditemukan. |

### Lihat Juga

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Mendapatkan info instance arsip.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran file arsip. |

### Nilai Kembalian

Informasi tentang instance arsip atau null jika format tidak terdeteksi.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *stream* bernilai null. |
| ArgumentException | *stream* tidak dapat di-seek. |

### Lihat Juga

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


