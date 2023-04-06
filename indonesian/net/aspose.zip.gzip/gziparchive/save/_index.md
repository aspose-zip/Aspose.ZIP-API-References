---
title: GzipArchive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: GzipArchive metode. Menyimpan arsip ke aliran yang disediakan.
type: docs
weight: 60
url: /id/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *outputStream* tidak dapat ditulis. |
| InvalidOperationException | Sumber belum diberikan. |

### Perkataan

*outputStream*harus dapat ditulis.

### Contoh

Menulis data terkompresi ke aliran respons http.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

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
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)


