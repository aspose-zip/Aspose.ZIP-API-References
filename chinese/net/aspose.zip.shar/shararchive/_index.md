---
title: Class SharArchive
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Shar.SharArchive 班级. 此类表示 shar 存档文件
type: docs
weight: 700
url: /zh/net/aspose.zip.shar/shararchive/
---
## SharArchive class

此类表示 shar 存档文件。

```csharp
public class SharArchive : IDisposable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | 初始化一个新的实例`SharArchive`类. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | 获取条目[`SharEntry`](../sharentry/)构成档案的类型. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | 将给定目录中的所有文件和目录递归添加到存档中。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | 在存档中创建单个条目。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | 按索引从条目列表中删除条目。 |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | 从条目列表中删除第一次出现的特定条目。 |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | 执行与释放、释放或重置非托管资源相关的应用程序定义的任务。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | 将存档保存到提供的流中。 |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | 将存档保存到提供的目标文件。 |

### 也可以看看

* 命名空间 [Aspose.Zip.Shar](../../aspose.zip.shar/)
* 部件 [Aspose.Zip](../../)


