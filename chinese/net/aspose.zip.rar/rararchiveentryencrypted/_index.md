---
title: Class RarArchiveEntryEncrypted
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Rar.RarArchiveEntryEncrypted 班级. 需要解密解压的zip入口
type: docs
weight: 330
url: /zh/net/aspose.zip.rar/rararchiveentryencrypted/
---
## RarArchiveEntryEncrypted class

需要解密解压的zip入口。

```csharp
public sealed class RarArchiveEntryEncrypted : RarArchiveEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | 获取压缩文件的大小。 |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | 获取创建日期和时间。 |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | 获取上次访问日期和时间。 |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | 获取上次修改日期和时间。 |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | 获取存档中条目的名称。 |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | 获取原始文件的大小。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | 打开用于提取的条目并提供具有解压缩条目内容的流。 |

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | 提取原始流的一部分时引发。 |

### 也可以看看

* class [RarArchiveEntry](../rararchiveentry/)
* 命名空间 [Aspose.Zip.Rar](../../aspose.zip.rar/)
* 部件 [Aspose.Zip](../../)


