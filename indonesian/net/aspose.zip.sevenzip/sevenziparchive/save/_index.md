---
title: SevenZipArchive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchive metode. Menyimpan arsip 7z ke aliran yang disediakan.
type: docs
weight: 80
url: /id/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Menyimpan arsip 7z ke aliran yang disediakan.

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
| InvalidOperationException | Encoder gagal mengompresi data. |

### Perkataan

*output* harus dapat dicari.

### Contoh

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
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

### Perkataan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama saat diambil dari. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

### Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)


