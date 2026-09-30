---
title: "类 ArjArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Arj.ArjArchive 类。此类表示 ARJ 存档文件"
type: docs
weight: 250
url: /zh/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

此类表示 ARJ 存档文件。

```csharp
public class ArjArchive : IArchive
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | 初始化 `ArjArchive` 类的新实例，并构建可从存档中提取的条目列表。 |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | 初始化 `ArjArchive` 类的新实例，并构建可从存档中提取的条目列表。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | 获取注释。 |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | 获取构成 ARJ 存档的 [`ArjEntryPlain`](../arjentryplain/) 类型的条目。 |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | 获取原始名称。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | 将所有条目提取到指定目录。 |

## 备注

仅支持以下压缩方法：

**Method**

**Explanation**

**0**

未压缩

**1**

LZ77 与自适应 Huffman 编码的组合。最佳压缩比。

**2**

LZ77 与自适应 Huffman 编码的组合。

**3**

LZ77 与自适应 Huffman 编码的组合。最佳速度。

### 另请参阅

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


