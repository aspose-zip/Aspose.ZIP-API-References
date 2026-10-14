---
title: "LhaArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LhaArchive 方法。将存档中的所有文件和目录提取到提供的目录。"
type: docs
weight: 40
url: /zh/net/aspose.zip.lha/lhaarchive/extracttodirectory/
---
## LhaArchive.ExtractToDirectory method

将存档中的所有文件和目录提取到提供的目录中。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | String | 放置提取文件的目录路径。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationDirectory* 为 null。 |
| PathTooLongException | 指定的路径、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| SecurityException | 调用者没有访问现有目录所需的权限。 |
| NotSupportedException | 如果目录不存在，路径包含冒号字符 (:)，且该冒号不是驱动器标签的一部分（"C:\"）。 |
| ArgumentException | *destinationDirectory* 为零长度字符串，仅包含空白，或包含一个或多个无效字符。您可以使用 System.IO.Path.GetInvalidPathChars 方法查询无效字符。-or- 路径前缀或仅包含冒号字符 (:)。 |
| IOException | 由 path 指定的目录是一个文件。-or- 网络名称未知。 |
| InvalidDataException | 提供了错误的密码。- 或 - 存档已损坏。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 当对象已被释放时抛出。 |

## 备注

如果目录不存在，将会创建它。

## 示例

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 另请参阅

* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


