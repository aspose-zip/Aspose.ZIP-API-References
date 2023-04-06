---
title: Bzip2Archive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2Archive metode. Menyimpan arsip ke aliran yang disediakan.
type: docs
weight: 50
url: /id/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |
| saveOptions | Bzip2SaveOptions | Opsi untuk menyimpan arsip bzip2. Jika tidak ditentukan, ukuran blok 900 Kb akan digunakan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Sumber data yang akan diarsipkan belum disediakan. |
| ArgumentException | *outputStream* tidak dapat ditulis. |
| UnauthorizedAccessException | Sumber file bersifat read-only atau berupa direktori. |
| DirectoryNotFoundException | Jalur sumber file yang ditentukan tidak valid, seperti berada di drive yang belum dipetakan. |
| IOException | Sumber File sudah terbuka. |

### Perkataan

*outputStream*harus dapat ditulis.

### Contoh

Menulis data terkompresi ke aliran respons http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Lihat juga

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| saveOptions | Bzip2SaveOptions | Opsi untuk menyimpan arsip bzip2. Jika tidak ditentukan, ukuran blok 900 Kb akan digunakan. |

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

Menulis data terkompresi ke file.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Lihat juga

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)


