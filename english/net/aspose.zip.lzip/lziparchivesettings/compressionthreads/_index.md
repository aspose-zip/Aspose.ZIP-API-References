---
title: LzipArchiveSettings.CompressionThreads
second_title: Aspose.ZIP for .NET API Reference
description: LzipArchiveSettings property. Gets or sets compression thread count. If the value is greater than 1 multithreading compression will be used
type: docs
weight: 70
url: /net/aspose.zip.lzip/lziparchivesettings/compressionthreads/
---
## LzipArchiveSettings.CompressionThreads property

Gets or sets compression thread count. If the value is greater than 1, multithreading compression will be used.

```csharp
public int CompressionThreads { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | The number of threads is more than 100. |

## Remarks

Do not set this number more than CPU cores.

### See Also

* class [LzipArchiveSettings](../)
* namespace [Aspose.Zip.Lzip](../../lziparchivesettings/)
* assembly [Aspose.Zip](../../../)


