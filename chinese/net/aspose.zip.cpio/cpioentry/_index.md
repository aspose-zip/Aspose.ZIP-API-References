---
title: CpioEntry
second_title: Aspose.ZIP for .NET API 参考
description: 表示 cpio 存档中的单个文件
type: docs
weight: 130
url: /zh/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

表示 cpio 存档中的单个文件。

```csharp
public sealed class CpioEntry
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory) { get; } | 获取一个值，该值指示该条目是否表示目录。 |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc) { get; } | 获取最后写入时间。 |
| [Length](../../aspose.zip.cpio/cpioentry/length) { get; } | 获取条目的长度（以字节为单位）。 |
| [Name](../../aspose.zip.cpio/cpioentry/name) { get; } | 获取存档中条目的名称。 |
| [Parent](../../aspose.zip.cpio/cpioentry/parent) { get; } | 获取条目所属的存档。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract#extract_1)(Stream) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.cpio/cpioentry/extract#extract)(string) | 通过提供的路径将条目提取到文件系统。 |
| [Open](../../aspose.zip.cpio/cpioentry/open)() | 打开条目以进行提取并提供带有条目内容的流。 |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring)() |  |

### 也可以看看

* 命名空间 [Aspose.Zip.Cpio](../../aspose.zip.cpio)
* 部件 [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->