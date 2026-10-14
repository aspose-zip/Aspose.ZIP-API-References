---
title: "类 AppleArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Apple.AppleArchive 类。此类表示 Apple Archive .aar 文件。使用它来创建 Apple Archive 文件"
type: docs
weight: 60
url: /zh/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

此类表示 Apple Archive（.aar）文件。可用于创建 Apple Archive 文件。

```csharp
public class AppleArchive : IArchive
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | 使用用于已组成条目的设置初始化 `AppleArchive` 类的新实例。 |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | 初始化 `AppleArchive` 类的新实例，并组成可从存档中提取的条目列表。 |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | 初始化 `AppleArchive` 类的新实例，并组成可从存档中提取的条目列表。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | 获取构成存档的条目。 |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | 获取一个值，指示存档是否使用固体压缩。在固体模式下，所有条目数据作为单一流进行压缩，无法单独提取条目。请改用 [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/)。 |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | 获取用于新组成条目的设置。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | 将给定目录中所有文件和子目录递归添加到存档中。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | 在存档中创建单个条目。 |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | 在存档中创建单个条目。 |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | 将存档中的所有文件提取到提供的目录。 |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | 将存档保存到提供的流中。 |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | 将存档保存到提供的目标文件中。 |

## 备注

Apple 和 Apple Archive 是 Apple Inc. 的商标。

### 另请参阅

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


