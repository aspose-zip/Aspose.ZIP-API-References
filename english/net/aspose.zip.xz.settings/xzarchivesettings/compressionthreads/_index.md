---
title: CompressionThreads
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 70
url: /net/aspose.zip.xz.settings/xzarchivesettings/compressionthreads/
---
## XzArchiveSettings.CompressionThreads property

Gets or sets compression thread count. If the value greater than 1, multithreading compression will be used.

```csharp
public int CompressionThreads { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | The number of threads is more than 100. |

### Remarks

Do not set this number more than CPU cores.

### See Also

* class [XzArchiveSettings](../../xzarchivesettings)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
