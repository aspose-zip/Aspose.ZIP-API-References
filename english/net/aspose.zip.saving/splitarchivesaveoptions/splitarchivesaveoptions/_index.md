---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP for .NET API Reference
description: SplitArchiveSaveOptions constructor. Instantiates settings for saving a multivolume ZIP archive
type: docs
weight: 10
url: /net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions(string, uint) {#constructor}

Instantiates settings for saving a multi-volume ZIP archive.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Name for volumes. May be with or without .zip extension. |
| segmentSize | UInt32 | Size of a volume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Segment size is less than 65536 bytes. |

## Remarks

Some volumes may be less than *segmentSize*. In most cases, the last segment will be less but rarely regular segments might be too.

Names of files will be as follows: *fileName*.z01, *fileName*.z02, ..., *fileName*.z(n-1), *fileName*.zip.

### See Also

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)

---

## SplitArchiveSaveOptions(uint) {#constructor_1}

Instantiates settings for saving a multi-volume ZIP archive.

```csharp
public SplitArchiveSaveOptions(uint segmentSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| segmentSize | UInt32 | Size of a volume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Segment size is less than 65536 bytes. |

## Remarks

Use this `SplitArchiveSaveOptions` instance without file name with [`SaveSplit`](../../../aspose.zip/archive/savesplit/) method.

Some volumes may be less than *segmentSize*. In most cases, the last segment will be less but rarely regular segments might be too.

### See Also

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


