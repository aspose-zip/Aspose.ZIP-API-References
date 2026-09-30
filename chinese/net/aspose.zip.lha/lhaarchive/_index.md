---
title: "类 LhaArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Lha.LhaArchive 类。此类表示一个 LHA .lzh 存档文件。"
type: docs
weight: 630
url: /zh/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

此类表示 LHA（.lzh）存档文件。

```csharp
public class LhaArchive : IArchive
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | 初始化 `LhaArchive` 类的新实例，并构建可从存档中提取的条目列表。 |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | 初始化 `LhaArchive` 类的新实例，并构建可从存档中提取的条目列表。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | 获取构成存档的 [`LhaArchiveEntry`](../lhaarchiveentry/) 类型的文件条目。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | 将存档中的所有文件和目录提取到提供的目录中。 |

## 备注

仅支持以下压缩方法：

**Method**

**Explanation**

**lh0**

未压缩

**lh4**

8 KiB 滑动字典和静态 Huffman

**lh5**

16 KiB 滑动字典和静态 Huffman

**lh6**

64 KiB 滑动字典和静态 Huffman

**lh7**

128 KiB 滑动字典和静态 Huffman

**lhx**

1 Mib 滑动字典和静态 Huffman

**lhd**

目录

### 另请参阅

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


