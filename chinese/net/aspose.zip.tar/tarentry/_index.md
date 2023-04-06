---
title: Class TarEntry
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Tar.TarEntry 班级. 表示 tar 存档中的单个文件
type: docs
weight: 740
url: /zh/net/aspose.zip.tar/tarentry/
---
## TarEntry class

表示 tar 存档中的单个文件。

```csharp
public class TarEntry : IArchiveFileEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [IsDirectory](../../aspose.zip.tar/tarentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [Length](../../aspose.zip.tar/tarentry/length/) { get; } | 获取以字节为单位的条目长度。 |
| [Name](../../aspose.zip.tar/tarentry/name/) { get; set; } | 获取或设置存档中条目的名称。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract_1)(Stream) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract)(string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.tar/tarentry/open/)() | 打开用于提取的条目并提供具有条目内容的流。 |

### 也可以看看

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.Tar](../../aspose.zip.tar/)
* 部件 [Aspose.Zip](../../)


