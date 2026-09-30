---
title: "SevenZipLZMA2CompressionSettings.CompressionThreads"
second_title: "Aspose.ZIP for .NET API 参考"
description: "SevenZipLZMA2CompressionSettings 属性。获取或设置压缩线程数。如果该值大于 1，将使用多线程压缩"
type: docs
weight: 20
url: /zh/net/aspose.zip.saving/sevenziplzma2compressionsettings/compressionthreads/
---
## SevenZipLZMA2CompressionSettings.CompressionThreads property

获取或设置压缩线程数。如果值大于 1，将使用多线程压缩。

```csharp
public int CompressionThreads { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 线程数大于 32。 |

## 备注

不要将此数字设置超过 CPU 核心数。

### 另请参阅

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


