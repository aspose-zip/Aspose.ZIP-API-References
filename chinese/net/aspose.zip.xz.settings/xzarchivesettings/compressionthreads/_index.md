---
title: "XzArchiveSettings.CompressionThreads"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XzArchiveSettings 属性。获取或设置压缩线程数。如果值大于 1，将使用多线程压缩"
type: docs
weight: 70
url: /zh/net/aspose.zip.xz.settings/xzarchivesettings/compressionthreads/
---
## XzArchiveSettings.CompressionThreads property

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

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


