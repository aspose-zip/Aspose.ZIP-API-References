---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchive metode. Menyimpan arsip multivolume ke direktori tujuan yang disediakan.
type: docs
weight: 90
url: /id/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Menyimpan arsip multi-volume ke direktori tujuan yang disediakan.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat segmen arsip dibuat. |
| options | SplitSevenZipArchiveSaveOptions | Opsi untuk menyimpan arsip, termasuk nama file. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Arsip ini dibuka dari sumber yang ada. |
| ArgumentNullException | *destinationDirectory* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses direktori. |
| ArgumentException | *destinationDirectory* berisi karakter yang tidak valid seperti ", &gt;, &lt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan melebihi panjang maksimum yang ditentukan sistem. |

### Perkataan

Metode ini menyusun beberapa (`N`) file namafile.7z.001, namafile.7z.002, ..., namafile.7z.(n).

Tidak dapat membuat arsip multi-volume yang ada.

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Lihat juga

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)


