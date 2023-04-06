---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry 班级. 表示 7z 存档中的单个文件
type: docs
weight: 670
url: /zh/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

表示 7z 存档中的单个文件。

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | 获取压缩文件的大小。 |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | 获取压缩或解压缩设置。 |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | 获取上次修改日期和时间。 |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | 获取存档中条目的名称。 |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | 获取原始文件的大小。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | 打开用于提取的条目并提供具有条目内容的流。 |

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | 在压缩原始流的一部分时引发。 |

### 评论

投一个`SevenZipArchiveEntry`实例到[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/)确定条目是否加密。

### 也可以看看

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 部件 [Aspose.Zip](../../)


