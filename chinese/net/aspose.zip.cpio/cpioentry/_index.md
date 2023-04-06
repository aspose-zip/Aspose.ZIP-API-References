---
title: Class CpioEntry
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Cpio.CpioEntry 班级. 表示 cpio 存档中的单个文件
type: docs
weight: 170
url: /zh/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

表示 cpio 存档中的单个文件。

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | 获取上次写入时间。 |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | 获取条目的字节长度。 |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | 获取存档中条目的名称。 |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | 获取条目所属的存档。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | 将条目提取到所提供的流中。 |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | 打开用于提取的条目并提供具有条目内容的流。 |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### 也可以看看

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 部件 [Aspose.Zip](../../)


