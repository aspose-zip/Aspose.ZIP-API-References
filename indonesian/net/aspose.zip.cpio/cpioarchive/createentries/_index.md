---
title: CpioArchive.CreateEntries
second_title: Aspose.ZIP untuk Referensi .NET API
description: CpioArchive metode. Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.
type: docs
weight: 30
url: /id/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceDirectory | String | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Contoh entri Cpio.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourceDirectory* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses*sourceDirectory*. |
| ArgumentException | *sourceDirectory* berisi karakter yang tidak valid seperti ", &lt;, &gt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. Jalur yang ditentukan, nama file, atau keduanya terlalu panjang. |
| IOException | *sourceDirectory* singkatan dari file, bukan direktori. |

### Contoh

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori untuk dikompres. |
| includeRootDirectory | Boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

### Nilai Pengembalian

Contoh entri Cpio.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *directory* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses*directory*. |
| IOException | *directory* singkatan dari file, bukan direktori. |

### Contoh

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)


