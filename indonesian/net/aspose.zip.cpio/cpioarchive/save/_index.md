---
title: CpioArchive.Save
second_title: Aspose.ZIP untuk Referensi .NET API
description: CpioArchive metode. Menyimpan arsip ke file tujuan yang disediakan.
type: docs
weight: 80
url: /id/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| cpioFormat | CpioFormat | Mendefinisikan format tajuk cpio. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *destinationFileName* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau beberapa karakter tidak valid seperti yang ditentukan oleh System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* adalah nol. |
| PathTooLongException | Yang ditentukan*destinationFileName*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| DirectoryNotFoundException | Yang ditentukan*destinationFileName* tidak valid, (misalnya, ada di drive yang belum dipetakan). |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| UnauthorizedAccessException | *destinationFileName* ditentukan file yang read-only dan akses tidak Baca.-atau- path ditentukan direktori.-atau- Penelepon tidak memiliki izin yang diperlukan. |
| NotSupportedException | *destinationFileName* dalam format yang tidak valid. |

### Perkataan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama saat diambil dari. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

### Contoh

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Lihat juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| cpioFormat | CpioFormat | Mendefinisikan format tajuk cpio. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah nol. |
| ArgumentException | *output* tidak dapat ditulis. - atau -*output* adalah aliran yang sama dengan tempat kami mengekstrak. - ATAU - Tidak mungkin menyimpan arsip di*cpioFormat* karena pembatasan format. |

### Perkataan

*output*harus dapat ditulis.

### Contoh

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Lihat juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)


