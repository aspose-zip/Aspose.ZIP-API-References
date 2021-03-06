---
title: SevenZipArchive
second_title: Aspose.ZIP for .NET API 参考
description: 这个类代表 7z 存档文件使用它来编写和提取 7z 档案
type: docs
weight: 540
url: /zh/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

这个类代表 7z 存档文件。使用它来编写和提取 7z 档案。

```csharp
public class SevenZipArchive : IDisposable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [SevenZipArchive](sevenziparchive#constructor)(SevenZipEntrySettings) | 使用其条目的可选设置初始化[`SevenZipArchive`](../sevenziparchive)类的新实例。 |
| [SevenZipArchive](sevenziparchive#constructor_1)(Stream) | 初始化[`SevenZipArchive`](../sevenziparchive)类的新实例，并且可以从存档中提取条目列表。 |
| [SevenZipArchive](sevenziparchive#constructor_2)(string) | 初始化[`SevenZipArchive`](../sevenziparchive)类的新实例，并且可以从存档中提取条目列表。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries) { get; } | 获取构成存档的[`SevenZipArchiveEntry`](../sevenziparchiveentry)类型的条目。 |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings) { get; } | 用于新添加的[`SevenZipArchiveEntry`](../sevenziparchiveentry)项目的压缩和加密设置。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries#createentries)(DirectoryInfo, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries#createentries_1)(string, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry#createentry_1)(string, Stream, SevenZipEntrySettings) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry#createentry_3)(string, string, bool, SevenZipEntrySettings) | 在存档中创建单个条目。 |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose)() | 执行与释放、释放或重置非托管资源相关的应用程序定义任务。 |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory)(string, string) | 将存档中的所有文件提取到提供的目录。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save#save)(Stream) | 将 7z 存档保存到提供的流中。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save#save_1)(string) | 将存档保存到提供的目标文件。 |

### 也可以看看

* 命名空间 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip)
* 部件 [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
