---
title: "LzxArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LzxArchive 方法。提取存档中的所有文件和目录到提供的目录"
type: docs
weight: 40
url: /zh/net/aspose.zip.lzx/lzxarchive/extracttodirectory/
---
## LzxArchive.ExtractToDirectory method

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
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidDataException | 提供了错误的密码。- 或 - 存档已损坏。 |
| NotSupportedException | 无效的压缩方法。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |

## 备注

如果目录不存在，将会创建它。

## 示例

```csharp
using (var archive = new LzxArchive("archive.lzx")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 另请参阅

* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


