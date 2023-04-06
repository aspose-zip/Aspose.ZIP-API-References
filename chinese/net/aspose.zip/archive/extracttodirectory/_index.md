---
title: Archive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API 参考
description: Archive 方法. 将存档中的所有文件提取到提供的目录中
type: docs
weight: 80
url: /zh/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

将存档中的所有文件提取到提供的目录中。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | String | 放置提取文件的目录的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *destinationDirectory*一片空白。 |
| PathTooLongException | 指定的路径、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| SecurityException | 调用者没有访问现有目录所需的权限。 |
| NotSupportedException | 如果目录不存在，则路径包含不属于驱动器标签（“C:\”）的冒号字符 (:)。 |
| ArgumentException | *destinationDirectory*是零长度字符串，仅包含空格，或包含一个或多个无效字符。您可以使用 System.IO.Path.GetInvalidPathChars 方法查询无效字符。 - 或 - 路径仅以冒号字符 (:) 为前缀或仅包含冒号字符 (:)。 |
| IOException | path 指定的目录是一个文件。 - 或 - 网络名称未知。 |
| InvalidDataException | 提供了错误的密码。 |

### 评论

如果该目录不存在，将创建它。

### 例子

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 也可以看看

* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)


