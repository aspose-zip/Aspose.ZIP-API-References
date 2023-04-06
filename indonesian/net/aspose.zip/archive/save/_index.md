---
title: Archive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Menyimpan arsip ke aliran yang disediakan.
type: docs
weight: 90
url: /id/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |
| saveOptions | ArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *outputStream* tidak dapat ditulis. |

### Perkataan

*outputStream*harus dapat ditulis.

### Contoh

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Lihat juga

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| saveOptions | ArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*destinationFileName* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*destinationFileName* ditolak. |
| PathTooLongException | Yang ditentukan*destinationFileName*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*destinationFileName* berisi titik dua (:) di tengah string. |

### Perkataan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama saat diambil dari. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

### Contoh

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Lihat juga

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


