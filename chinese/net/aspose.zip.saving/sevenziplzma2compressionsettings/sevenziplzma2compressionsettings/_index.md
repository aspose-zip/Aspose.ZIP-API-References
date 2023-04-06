---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: SevenZipLZMA2CompressionSettings 构造函数. 实例化 7z 存档中 LZMA2 压缩方法的设置
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

实例化 7z 存档中 LZMA2 压缩方法的设置。

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

字典越大，压缩率通常越好，但比未压缩数据大的字典是对 RAM 的浪费。

### 也可以看看

* class [SevenZipLZMA2CompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

实例化 7z 存档中 LZMA2 压缩方法的设置。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dictionarySize | Int32 | 历史缓冲区的大小，必须在 4096 和 1073741824 之间。 |
| fastBytes | Int32 | 控制 LZMA2 压缩器使用的快速字节数。较大数量的快速字节可以以压缩速度为代价提供更好的压缩比。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize*太大或太小，或*fastBytes*太大或太小。 |

### 评论

字典越大，压缩率通常越好，但比未压缩数据大的字典是对 RAM 的浪费。

### 也可以看看

* class [SevenZipLZMA2CompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 部件 [Aspose.Zip](../../../)


