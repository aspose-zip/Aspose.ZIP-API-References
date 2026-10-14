---
title: "CpioArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "CpioArchive metode. Menyimpan arsip ke file tujuan yang disediakan"
type: docs
weight: 80
url: /id/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| cpioFormat | CpioFormat | Mendefinisikan format header cpio. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destinationFileName* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid sebagaimana didefinisikan oleh System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* bernilai null. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| DirectoryNotFoundException | *destinationFileName* yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| UnauthorizedAccessException | *destinationFileName* Ditentukan file bersifat read-only dan akses tidak dapat dibaca. -or- path menunjuk ke direktori. -or- Pemanggil tidak memiliki izin yang diperlukan. |
| NotSupportedException | *destinationFileName* berada dalam format yang tidak valid. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

## Contoh

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Lihat Juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| cpioFormat | CpioFormat | Mendefinisikan format header cpio. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis. - or - *output* adalah aliran yang sama yang kami ekstrak. - OR - Tidak mungkin menyimpan arsip dalam *cpioFormat* karena pembatasan format. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

*output* must be writable.

## Contoh

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

### Lihat Juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


