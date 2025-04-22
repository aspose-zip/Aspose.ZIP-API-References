---
title: SevenZipLZMA2CompressionSettings.CompressionThreads
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipLZMA2CompressionSettings property. Gets or sets compression thread count. If the value is greater than 1 multithreading compression will be used
type: docs
weight: 20
url: /net/aspose.zip.saving/sevenziplzma2compressionsettings/compressionthreads/
---
## SevenZipLZMA2CompressionSettings.CompressionThreads property

Gets or sets compression thread count. If the value is greater than 1, multithreading compression will be used.

```csharp
public int CompressionThreads { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | The number of threads is higher than 32. |

## Remarks

Do not set this number more than CPU cores.

### See Also

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


