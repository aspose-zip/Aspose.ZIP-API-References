---
title: "SevenZipArchive.SaveSplit"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SevenZipArchive. Menyimpan arsip multivolume ke direktori tujuan yang diberikan"
type: docs
weight: 90
url: /id/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Menyimpan arsip multi-volume ke direktori tujuan yang disediakan.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat segmen arsip akan dibuat. |
| opsi | SplitSevenZipArchiveSaveOptions | Opsi untuk menyimpan arsip, termasuk nama file. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationDirectory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori. |
| ArgumentException | *destinationDirectory* berisi karakter tidak valid seperti \", &gt;, &lt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

## Catatan

Metode ini menyusun beberapa file (`n`) seperti filename.7z.001, filename.7z.002, ..., filename.7z.(n).

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Lihat Juga

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


