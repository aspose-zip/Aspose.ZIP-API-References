---
title: SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: 在 7z 存档中实例化 LZMA2 压缩方法的设置
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings constructor

在 7z 存档中实例化 LZMA2 压缩方法的设置。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dictionarySize | Int32 | 历史缓冲区的大小，必须在 4096 和 1073741824 之间。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize*太大或太小。 |

### 评论

字典越大越好压缩比通常是，但是大于未压缩数据的字典是RAM的浪费。

### 也可以看看

* class [SevenZipLZMA2CompressionSettings](../../sevenziplzma2compressionsettings)
* 命名空间 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
