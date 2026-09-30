---
title: "WimArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "WimArchive 方法。按路径将存档提取到文件。"
type: docs
weight: 90
url: /zh/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

将存档提取到指定路径的文件中。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | String | 放置提取文件的目录路径。 |

### Return Value

已提取文件的信息。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *destinationDirectory* 为 null |
| PathTooLongException | 指定的路径、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| SecurityException | 调用者没有访问现有目录所需的权限。 |
| NotSupportedException | 如果目录不存在，路径包含冒号字符 (:) 且不是驱动器标签的一部分 (\"C:\\") - 或者 - WIM 存档是多部分的。 |
| ArgumentException | 路径是零长度字符串，仅包含空白，或包含一个或多个无效字符。您可以使用 System.IO.Path.GetInvalidPathChars 方法查询无效字符。-或- 路径以前缀或仅包含冒号字符 (:)。 |
| IOException | 由 path 指定的目录是一个文件。-or- 网络名称未知。 |
| InvalidDataException | 存档已损坏。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |

### 另请参阅

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


