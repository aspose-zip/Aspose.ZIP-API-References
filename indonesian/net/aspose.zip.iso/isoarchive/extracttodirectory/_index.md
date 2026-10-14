---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode IsoArchive. Mengekstrak semua entri ke direktori yang ditentukan"
type: docs
weight: 60
url: /id/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

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
| InvalidOperationException | Dilempar ketika arsip berada dalam mode penyuntingan. |
| ArgumentNullException | Dilempar ketika *destinationDirectory* bernilai null. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat Juga

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


