---
title: "XzArchiveSettings.XzArchiveSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor XzArchiveSettings. Menginisialisasi instance baru dari kelas XzArchiveSettings menggunakan kompresi LZMA2 tunggal"
type: docs
weight: 10
url: /id/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`XzArchiveSettings`](../) menggunakan kompresi LZMA2 tunggal.

```csharp
public XzArchiveSettings()
```

## Catatan

Kamus default pada filter LZMA2 berukuran 16 megabyte, ukuran blok default 64 megabyte, tipe checksum default adalah CRC32.

### Lihat Juga

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Menginisialisasi instance baru dari kelas [`XzArchiveSettings`](../) dengan parameter khusus.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filter (kompresor) yang akan diterapkan secara berurutan untuk membuat [`XzArchive`](../../../aspose.zip.xz/xzarchive/). Bisa berupa satu [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) atau pasangan [`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) dan [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |
| blockSize | Int64 | Ukuran blok arsip xz. |
| checkType | XzCheckType | Tipe perhitungan checksum untuk data yang tidak terkompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* bernilai negatif. |
| ArgumentNullException | *filters* bernilai null |
| ArgumentException | *filters* memiliki kurang dari satu atau lebih dari dua filter, atau filter terakhir bukan [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

## Contoh

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

### Lihat Juga

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


