---
title: "类 EggEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Egg.EggEntry 类。表示 EGG 存档中包含所有元数据的文件条目"
type: docs
weight: 470
url: /zh/net/aspose.zip.egg/eggentry/
---
## EggEntry class

表示 EGG 存档中包含所有元数据的文件条目。

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | 获取条目的压缩大小。 |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | 获取一个值，指示此条目是否表示目录。 |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | 获取或设置最后修改日期和时间。 |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | 获取存档中条目的名称。 |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | 获取条目的未压缩大小。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | 按提供的路径将条目提取到文件系统中。 |
| [Open](../../aspose.zip.egg/eggentry/open/)() | 打开条目以进行提取，并提供包含解压后条目内容的流。 |

### 另请参阅

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


