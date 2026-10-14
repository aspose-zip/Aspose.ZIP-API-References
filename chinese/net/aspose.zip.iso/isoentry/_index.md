---
title: "类 IsoEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Iso.IsoEntry 类。表示 ISO 存档中的条目文件或目录。"
type: docs
weight: 580
url: /zh/net/aspose.zip.iso/isoentry/
---
## IsoEntry class

表示 ISO 存档中的条目（文件或目录）。

```csharp
public abstract class IsoEntry : IArchiveFileEntry
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [IsDirectory](../../aspose.zip.iso/isoentry/isdirectory/) { get; } | 获取指示该条目是否为目录的值。 |
| [Length](../../aspose.zip.iso/isoentry/length/) { get; } | 获取或设置创建日期和时间。 |
| [ModificationTime](../../aspose.zip.iso/isoentry/modificationtime/) { get; } | 获取或设置最后修改日期和时间。 |
| [Name](../../aspose.zip.iso/isoentry/name/) { get; } | 获取条目的名称。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract_1)(Stream) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract)(string) | 按提供的路径将条目提取到文件系统中。 |
| override [ToString](../../aspose.zip.iso/isoentry/tostring/)() | 返回表示当前条目的字符串。 |

### 另请参阅

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


