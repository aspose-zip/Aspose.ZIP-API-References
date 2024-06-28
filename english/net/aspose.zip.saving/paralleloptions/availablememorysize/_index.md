---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP for .NET API Reference
description: ParallelOptions property. Gets or sets memory estimate in megabytes available to accomodate compressed entries without swap to disk. This value only makes sense if ParallelCompressInMemory setting is in Auto mode
type: docs
weight: 20
url: /net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Gets or sets memory estimate in megabytes available to accomodate compressed entries without swap to disk. This value only makes sense if [`ParallelCompressInMemory`](../parallelcompressinmemory/) setting is in Auto mode.

```csharp
public int AvailableMemorySize { get; set; }
```

## Remarks

This value is used to calculate biggest size of entry that can be compressed in parallel with others. All entries above the calculated threshold will be compressed sequentially. It is safe to have `AvailableMemorySize` property as big as free RAM and even bigger. By default it is assumed you have at least 200MB per CPU core.

### See Also

* class [ParallelOptions](../)
* namespace [Aspose.Zip.Saving](../../paralleloptions/)
* assembly [Aspose.Zip](../../../)


