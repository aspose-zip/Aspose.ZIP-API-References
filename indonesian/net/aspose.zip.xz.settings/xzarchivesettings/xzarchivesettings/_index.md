---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzArchiveSettings konstruktor. Menginisialisasi instance baru dariXzArchiveSettings kelas menggunakan kompresi LZMA2 tunggal.
type: docs
weight: 10
url: /id/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Menginisialisasi instance baru dari[`XzArchiveSettings`](../) kelas menggunakan kompresi LZMA2 tunggal.

```csharp
public XzArchiveSettings()
```

### Perkataan

Kamus default dalam ukuran filter LZMA2 sama dengan 16 megabyte, ukuran blok default sama dengan 64 megabyte, tipe checksum default adalah CRC32.

### Lihat juga

* class [XzArchiveSettings](../)
* ruang nama [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* perakitan [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Menginisialisasi instance baru dari[`XzArchiveSettings`](../) kelas dengan parameter khusus.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filter (kompresor) yang akan diterapkan secara berurutan untuk dibuat[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Itu bisa tunggal[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) atau sepasang[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) Dan[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Ukuran blok arsip xz. |
| checkType | XzCheckType | Jenis perhitungan checksum untuk data yang tidak terkompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* negatif. |
| ArgumentNullException | *filters* adalah nol |
| ArgumentException | *filters* memiliki kurang dari satu atau lebih dari dua filter, atau filter terakhir tidak[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Contoh

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Lihat juga

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* ruang nama [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* perakitan [Aspose.Zip](../../../)


