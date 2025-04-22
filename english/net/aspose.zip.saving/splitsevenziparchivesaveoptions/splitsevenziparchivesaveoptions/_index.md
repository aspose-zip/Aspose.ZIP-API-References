---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP for .NET API Reference
description: SplitSevenZipArchiveSaveOptions constructor. Instantiates settings for saving a multivolume 7z archive
type: docs
weight: 10
url: /net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instantiates settings for saving a multi-volume 7z archive.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Name for volumes. May be with or without .7z extension. |
| segmentSize | UInt32 | Size of volume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* is less than 100. |

## Remarks

Some volumes may be less than *segmentSize*. In most cases, the last segment will be less but rarely regular segments might be too.

Names of files will be as follows: *fileName*.7z.001, *fileName*.7z.002, ..., *fileName*.7z.(n).

### See Also

* class [SplitSevenZipArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


