---
title: Class CpioArchive
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Cpio.CpioArchive 班级. 这个类表示 cpio 归档文件
type: docs
weight: 160
url: /zh/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

这个类表示 cpio 归档文件。

```csharp
public class CpioArchive : IArchive
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | 初始化一个新的实例`CpioArchive`类. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | 初始化一个新的实例`CpioArchive`可以从存档中提取类和组合条目列表。 |
| [CpioArchive](cpioarchive/#constructor_2)(string) | 初始化一个新的实例`CpioArchive`可以从存档中提取类和组合条目列表。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | 获取条目[`CpioEntry`](../cpioentry/)构成档案的类型. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | 在存档中创建单个条目。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | 从条目列表中删除第一次出现的特定条目。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | 按索引从条目列表中删除条目。 |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | 执行与释放、释放或重置非托管资源相关的应用程序定义的任务。 |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | 将存档中的所有文件提取到提供的目录中。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | 将存档保存到提供的流中。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | 将存档保存到提供的目标文件。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | 使用 gzip 压缩将存档保存到流中。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | 使用 gzip 压缩按路径将存档保存到文件。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | 使用 xz 压缩将存档保存到流中。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | 将压缩包按路径保存到 xz 压缩路径下。 |

### 也可以看看

* interface [IArchive](../../aspose.zip/iarchive/)
* 命名空间 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 部件 [Aspose.Zip](../../)


