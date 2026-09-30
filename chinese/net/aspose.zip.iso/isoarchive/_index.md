---
title: "类 IsoArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.Iso.IsoArchive 类。表示 ISO 9660 ISO 存档。"
type: docs
weight: 570
url: /zh/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

表示 ISO 存档 (ISO 9660)。

```csharp
public sealed class IsoArchive : IArchive
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | 初始化 `IsoArchive` 类的新实例，并创建一个空的 ISO 存档，以便添加新文件和目录。 |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | 初始化 `IsoArchive` 类的新实例，并构建一个可从存档中提取的条目列表。 |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | 初始化 `IsoArchive` 类的新实例，并构建一个可从存档中提取的条目列表。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | 获取构成存档的 [`IsoEntry`](../isoentry/) 类型的条目。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | 向 ISO 镜像添加目录。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | 向 ISO 镜像添加文件。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | 向 ISO 镜像添加文件。 |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | 向 ISO 镜像添加文件。 |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | 将所有条目提取到指定目录。 |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | 将 ISO 镜像保存到指定的流。 |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | 将 ISO 镜像保存到指定路径。 |

### 另请参阅

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


