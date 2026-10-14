---
title: "类 AppleArchiveEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Apple.AppleArchiveEntry 类。表示 AppleArchive 中的文件系统条目"
type: docs
weight: 70
url: /zh/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

表示 [`AppleArchive`](../applearchive/) 中的文件系统条目。

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | 获取一个值，指示该条目是否表示目录。 |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | 获取一个值，指示该条目是否表示符号链接。 |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | 获取该条目的未压缩长度（字节）。 |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | 获取条目在归档中的路径。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | 按提供的路径将条目提取到文件系统中。 |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | 打开条目以进行提取，并提供包含条目内容的流。 |

## 备注

此类的实例可以表示从现有 Apple Archive 解析出的普通文件、目录或符号链接，或添加到正在创建的归档中的文件或目录。

### 另请参阅

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


