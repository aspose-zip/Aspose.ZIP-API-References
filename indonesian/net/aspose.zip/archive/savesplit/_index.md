---
title: Archive.SaveSplit
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Menyimpan arsip multivolume ke direktori tujuan yang disediakan.
type: docs
weight: 100
url: /id/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Menyimpan arsip multi-volume ke direktori tujuan yang disediakan.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat segmen arsip dibuat. |
| options | SplitArchiveSaveOptions | Opsi untuk menyimpan arsip, termasuk nama file. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Arsip ini dibuka dari sumber yang ada. |
| NotSupportedException | Arsip ini dikompresi dengan metode XZ dan dienkripsi. |
| ArgumentNullException | *destinationDirectory* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses direktori. |
| ArgumentException | *destinationDirectory* berisi karakter yang tidak valid seperti ", &gt;, &lt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan melebihi panjang maksimum yang ditentukan sistem. |

### Perkataan

Metode ini menyusun beberapa (`N`) file namafile.z01, namafile.z02, ..., namafile.z(n-1), namafile.zip.

Tidak dapat membuat arsip multi-volume yang ada.

### Contoh

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Lihat juga

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


