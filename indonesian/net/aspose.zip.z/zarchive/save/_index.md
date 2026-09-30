---
title: "ZArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ZArchive. Menyimpan arsip xz ke stream yang diberikan"
type: docs
weight: 50
url: /id/net/aspose.zip.z/zarchive/save/
---
## Save(Stream, ZArchiveSaveOptions) {#save}

Menyimpan arsip xz ke stream yang disediakan.

```csharp
public void Save(Stream output, ZArchiveSaveOptions settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| pengaturan | ZArchiveSaveOptions | Pengaturan opsional untuk komposisi arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *output* tidak mendukung pencarian. |
| ArgumentNullException | *output* adalah null. |

## Catatan

*output* must be seekable.

## Contoh

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### Lihat Juga

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZArchiveSaveOptions) {#save_1}

Menyimpan arsip Z ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, ZArchiveSaveOptions settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | +Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| pengaturan | ZArchiveSaveOptions | Pengaturan opsional untuk komposisi arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *destinationFileName* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *destinationFileName* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *destinationFileName* ditolak. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *destinationFileName* berisi tanda titik dua (:) di tengah string. |
| IOException | Terjadi kesalahan I/O saat membuka file. |

## Contoh

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Lihat Juga

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


