---
title: Archive.CreateEntries
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.
type: docs
weight: 40
url: /id/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Lihat juga

* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceDirectory | String | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Arsip dengan entri disusun.

### Contoh

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Lihat juga

* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


