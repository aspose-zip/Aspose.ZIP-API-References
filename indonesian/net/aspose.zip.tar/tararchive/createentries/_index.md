---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.
type: docs
weight: 70
url: /id/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Arsip dengan entri disusun.

### Contoh

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceDirectory | String | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Arsip dengan entri disusun.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourceDirectory* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses*sourceDirectory*. |
| ArgumentException | *sourceDirectory* berisi karakter yang tidak valid seperti ", &lt;, &gt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. Jalur yang ditentukan, nama file, atau keduanya terlalu panjang. |

### Contoh

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


