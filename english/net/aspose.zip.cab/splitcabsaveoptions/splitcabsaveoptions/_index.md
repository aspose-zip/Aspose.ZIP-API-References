---
title: SplitCabSaveOptions.SplitCabSaveOptions
second_title: Aspose.ZIP for .NET API Reference
description: SplitCabSaveOptions constructor. Instantiates settings for saving a multivolume CAB archive
type: docs
weight: 10
url: /net/aspose.zip.cab/splitcabsaveoptions/splitcabsaveoptions/
---
## SplitCabSaveOptions constructor

Instantiates settings for saving a multi-volume CAB archive.

```csharp
public SplitCabSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Name for volumes. May be with or without .cab extension. |
| segmentSize | UInt32 | Size of a volume, from 65536 to 2147483647 bytes inclusive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *fileName* is null. |
| ArgumentException | *fileName* is empty, contains a path, non-ASCII characters, or characters not valid in a cabinet name. |
| ArgumentOutOfRangeException | Segment size is outside the supported range. |

## Remarks

Names of files will be as follows: *fileName*1.cab, *fileName*2.cab, ..., *fileName*`n`.cab.

All segments except the last one will normally have exactly *segmentSize* bytes.

### See Also

* class [SplitCabSaveOptions](../)
* namespace [Aspose.Zip.Cab](../../splitcabsaveoptions/)
* assembly [Aspose.Zip](../../../)


