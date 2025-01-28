---
title: Class ParallelOptions
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Saving.ParallelOptions class. Options for parallel compression
type: docs
weight: 610
url: /net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Options for parallel compression.

```csharp
public class ParallelOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Gets or sets memory estimate in megabytes available to accomodate compressed entries without swap to disk. This value only makes sense if [`ParallelCompressInMemory`](./parallelcompressinmemory/) setting is in Auto mode. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Gets or sets value indicating how parallel approach to be used. |

## Remarks

These options manage simultaneous compression by several CPU cores.

## Examples

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = ParallelCompressionMode.Auto, AvailableMemorySize = 4000 } });
}
```

### See Also

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


