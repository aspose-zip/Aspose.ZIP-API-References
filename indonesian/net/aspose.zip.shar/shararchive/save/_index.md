---
title: "SharArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SharArchive. Menyimpan arsip ke file tujuan yang diberikan"
type: docs
weight: 70
url: /id/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destinationFileName* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid sebagaimana didefinisikan oleh System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* bernilai null. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| DirectoryNotFoundException | *destinationFileName* yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| UnauthorizedAccessException | *destinationFileName* menentukan file yang hanya-baca dan akses tidak dapat dibaca.-or- jalur menentukan direktori.-or- Pemanggil tidak memiliki izin yang diperlukan. |
| NotSupportedException | *destinationFileName* berada dalam format yang tidak valid. |
| FileNotFoundException | Berkas tidak ditemukan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip ini dibuka untuk ekstraksi. |

## Catatan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

## Contoh

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis. - atau - *output* adalah aliran yang sama kita ekstrak darinya. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip ini dibuka untuk ekstraksi. |

## Catatan

*output* must be writable.

## Contoh

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


