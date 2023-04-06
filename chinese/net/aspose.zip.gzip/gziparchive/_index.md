---
title: Class GzipArchive
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Gzip.GzipArchive 班级. 此类代表 gzip 存档文件用它来编写或提取 gzip archives.
type: docs
weight: 210
url: /zh/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

此类代表 gzip 存档文件。用它来编写或提取 gzip archives.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | 初始化一个新的实例`GzipArchive`准备压缩的类. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | 初始化一个新的实例`GzipArchive`准备解压的类. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | 初始化一个新的实例`GzipArchive`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | 原始文件的名称. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | 执行与释放、释放或重置非托管资源相关的应用程序定义的任务。 |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | 将存档提取到提供的流中。 |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | 打开存档进行提取并提供包含存档内容的流。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | 将存档保存到提供的流中。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | 将存档保存到提供的目标文件。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | 设置要在存档中压缩的内容。 |

### 评论

Gzip 压缩算法基于 DEFLATE 算法，它是 LZ77 和霍夫曼编码的结合。

### 也可以看看

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* 部件 [Aspose.Zip](../../)


