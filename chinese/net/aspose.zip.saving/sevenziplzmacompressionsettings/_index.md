---
title: Class SevenZipLZMACompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Saving.SevenZipLZMACompressionSettings 班级. 7z 存档中 LZMA 压缩方法的设置
type: docs
weight: 580
url: /zh/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

7z 存档中 LZMA 压缩方法的设置。

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | Dictionary (history buffer) size 表示最近处理的未压缩数据在内存中保留了多少字节。 如果未设置，将相应地选择条目大小。 |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | 获取压缩或解压方法。 |

### 评论

Lempel-Ziv-Markov 链算法 (LZMA) 是一种用于执行无损数据压缩的算法。 该算法使用有点类似于 LZ77 算法的字典压缩方案，具有高压缩比和可变压缩字典大小的特点。

查看更多：https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm

### 也可以看看

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* 命名空间 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 部件 [Aspose.Zip](../../)


