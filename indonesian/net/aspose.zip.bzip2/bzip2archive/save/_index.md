---
title: "Bzip2Archive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Bzip2Archive. Menyimpan arsip ke aliran yang diberikan."
type: docs
weight: 60
url: /id/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |
| saveOptions | Bzip2SaveOptions | Opsi untuk menyimpan arsip bzip2. Jika tidak ditentukan, ukuran blok 900 Kb akan digunakan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Sumber data yang akan diarsipkan belum disediakan. |
| ArgumentException | *outputStream* tidak dapat ditulis. |
| UnauthorizedAccessException | Sumber file bersifat read-only atau merupakan direktori. |
| DirectoryNotFoundException | Jalur sumber file yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Sumber File sudah terbuka. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

*outputStream* must be writable.

## Contoh

Tulis data terkompresi ke aliran respons http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Lihat Juga

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| saveOptions | Bzip2SaveOptions | Opsi untuk menyimpan arsip bzip2. Jika tidak ditentukan, ukuran blok 900 Kb akan digunakan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *destinationFileName* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *destinationFileName* ditolak. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *destinationFileName* berisi tanda titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Sumber data yang akan diarsipkan belum disediakan. |

## Contoh

Menulis data terkompresi ke file.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Lihat Juga

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


