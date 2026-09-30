---
title: "类 AlzEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Alz.AlzEntry 类。表示 ALZ 存档中具有全部元数据的文件条目"
type: docs
weight: 30
url: /zh/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

表示 ALZ 存档中包含所有元数据的文件条目。

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | 文件数据的压缩大小（字节）。 |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | 如果此条目表示目录，则返回 true。 |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | 文件名（不含路径）。 |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | 文件数据的未压缩大小（字节）。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | 按提供的路径将条目提取到文件系统中。 |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | 打开条目以进行提取，并提供包含解压后条目内容的流。 |

### 另请参阅

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


