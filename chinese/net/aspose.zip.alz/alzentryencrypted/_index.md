---
title: "类 AlzEntryEncrypted"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Alz.AlzEntryEncrypted 类。需要在解压缩前解密的 ALZ 条目"
type: docs
weight: 40
url: /zh/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

在解压缩之前需要解密的 ALZ 条目。

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
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
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | 将条目提取到提供的流中。 |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | 按提供的路径将条目提取到文件系统中。 |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | 打开条目以进行提取，并提供包含解压后条目内容的流。 |

### 另请参阅

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


