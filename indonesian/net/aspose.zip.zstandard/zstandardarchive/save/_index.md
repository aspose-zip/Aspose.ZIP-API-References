---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "ZstandardArchive metode. Menyimpan arsip ke aliran yang disediakan."
type: docs
weight: 60
url: /id/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |
| pengaturan | ZstandardSaveOptions | Pengaturan opsional untuk komposisi arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *outputStream* tidak dapat ditulis. |
| InvalidOperationException | Sumber belum disediakan. |

## Catatan

*outputStream* must be writable.

## Contoh

Tulis data terkompresi ke aliran respons http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Lihat Juga

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| pengaturan | ZstandardSaveOptions | Pengaturan opsional untuk komposisi arsip. |

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
| Exception | Dilemparkan ketika terjadi kesalahan runtime. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| InvalidOperationException | Sumber belum disediakan. |

## Contoh

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Lihat Juga

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | FileInfo | FileInfo, yang akan dibuka sebagai aliran tujuan. |
| pengaturan | ZstandardSaveOptions | Pengaturan opsional untuk komposisi arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk membuka *destination*. |
| ArgumentException | Path file kosong atau hanya berisi spasi. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau merupakan direktori. |
| ArgumentNullException | *destination* bernilai null. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| InvalidOperationException | Sumber belum disediakan. |

## Contoh

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Lihat Juga

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


