---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArjArchive. Mengekstrak semua entri ke direktori yang ditentukan."
type: docs
weight: 60
url: /id/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

Mengekstrak semua entri ke direktori yang ditentukan.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Direktori tempat mengekstrak entri. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | Dilempar ketika *destinationDirectory* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| NotImplementedException | Entri dikompresi dengan metode 4. |

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


