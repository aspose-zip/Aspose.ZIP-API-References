---
title: XzArchiveSettings
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings constructor (1 of 2)

Initializes a new instance of the [`XzArchiveSettings`](../../xzarchivesettings) class using single LZMA2 compression.

```csharp
public XzArchiveSettings()
```

### Remarks

Default dictionary in LZMA2 filter size equals to 16 megabyte, default block size equals to 64 megabytes, default checksum type is CRC32.

### See Also

* class [XzArchiveSettings](../../xzarchivesettings)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings)
* assembly [Aspose.Zip](../../../)

---

## XzArchiveSettings constructor (2 of 2)

Initializes a new instance of the [`XzArchiveSettings`](../../xzarchivesettings) class with custom parameters.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filters (compressors) to be sequentially applied to create [`XzArchive`](../../../aspose.zip.xz/xzarchive). It can be either single [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings) or pair of [`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings) and [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings) |
| blockSize | Int64 | Size xz archive block. |
| checkType | XzCheckType | Type of checksum calculation for uncompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* is negative. |
| ArgumentNullException | *filters* is null |
| ArgumentException | *filters* has less than one or more than two filter, or last filter is not [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings). |

### Examples

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

### See Also

* class [XzFilterSettings](../../xzfiltersettings)
* enum [XzCheckType](../../xzchecktype)
* class [XzArchiveSettings](../../xzarchivesettings)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->