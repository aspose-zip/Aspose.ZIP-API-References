---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.ArchiveEntryPlain 班级. 需要在不加密的情况下压缩或在不解密的情况下解压缩的 Zip 条目
type: docs
weight: 40
url: /zh/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

需要在不加密的情况下压缩或在不解密的情况下解压缩的 Zip 条目。

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | 获取存档中条目的注释。 |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | 获取压缩文件的大小。 |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | 获取压缩或解压缩设置。 |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | 获取或设置上次修改日期和时间。 |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | 获取存档中条目的名称。 |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | 获取原始文件的大小。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip/archiveentry/open/)(string) | 打开用于提取的条目并提供具有解压缩条目内容的流。 |

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | 在压缩原始流的一部分时引发。 |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | 提取原始流的一部分时引发。 |

### 也可以看看

* class [ArchiveEntry](../archiveentry/)
* 命名空间 [Aspose.Zip](../../aspose.zip/)
* 部件 [Aspose.Zip](../../)


