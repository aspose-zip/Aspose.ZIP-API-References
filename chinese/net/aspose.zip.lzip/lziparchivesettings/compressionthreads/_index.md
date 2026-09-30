---
title: "LzipArchiveSettings.CompressionThreads"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LzipArchiveSettings 属性。获取或设置压缩线程数。如果该值大于 1，将使用多线程压缩"
type: docs
weight: 70
url: /zh/net/aspose.zip.lzip/lziparchivesettings/compressionthreads/
---
## LzipArchiveSettings.CompressionThreads property

获取或设置压缩线程数。如果值大于 1，将使用多线程压缩。

```csharp
public int CompressionThreads { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 线程数超过 100。 |

## 备注

不要将此数字设置超过 CPU 核心数。

### 另请参阅

* class [LzipArchiveSettings](../)
* namespace [Aspose.Zip.Lzip](../../lziparchivesettings/)
* assembly [Aspose.Zip](../../../)


