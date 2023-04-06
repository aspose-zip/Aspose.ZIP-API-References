---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchive metode. Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.
type: docs
weight: 40
url: /id/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Arsip dengan entri disusun.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| DirectoryNotFoundException | Jalan menuju*directory* tidak valid, seperti berada di drive yang belum dipetakan. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses*directory*. |

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceDirectory | String | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Arsip dengan entri disusun.

### Contoh

Buat arsip 7z dengan kompresi LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)


