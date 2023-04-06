---
title: XzArchive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzArchive metode. Menyimpan arsip xz ke aliran yang disediakan.
type: docs
weight: 40
url: /id/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

Menyimpan arsip xz ke aliran yang disediakan.

```csharp
public void Save(Stream output)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *output* tidak mendukung pencarian. |
| ArgumentNullException | *output* adalah nol. |

### Perkataan

*output* harus dapat dicari.

### Contoh

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Menyimpan arsip xz ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*destinationFileName* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*destinationFileName* ditolak. |
| PathTooLongException | Yang ditentukan*destinationFileName*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*destinationFileName* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)


