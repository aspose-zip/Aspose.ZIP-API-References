---
title: Class WimFileEntry
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Wim.WimFileEntry 班级. 表示 wim 存档中的单个文件
type: docs
weight: 790
url: /zh/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

表示 wim 存档中的单个文件。

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | 获取文件或目录的备用数据流的名称。 |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | 获取条目所属的存档。 |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | 获取上次更改文件或目录的时间。 |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | 获取文件或目录的创建时间。 |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | 获取文件或目录属性。 |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | 获取图像中条目的完整路径。 |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | 获取文件或目录的硬链接 ID。 |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | 获取文件或目录是否有其他名称。 |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | 获取条目所属的图像。 |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | 获取文件或目录的最后访问时间。 |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | 获取文件或目录的修改时间。 |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | 获取条目的字节长度。 |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | 获取图像中条目的名称。 |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | 获取条目所属的父目录。 |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | 获取图像中条目的简称。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | 打开用于提取的条目并提供具有条目内容的流。 |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### 也可以看看

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.Wim](../../aspose.zip.wim/)
* 部件 [Aspose.Zip](../../)


