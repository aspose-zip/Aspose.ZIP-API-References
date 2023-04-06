---
title: CabArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API 参考
description: CabArchive 方法. 将存档中的所有文件提取到提供的目录中
type: docs
weight: 40
url: /zh/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

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
| ArgumentNullException | 路径为空 |
| PathTooLongException | 指定的路径、文件名或两者都超过了系统定义的最大长度。 |
| SecurityException | 调用者没有访问现有目录所需的权限。 |
| NotSupportedException | 如果目录不存在，则路径包含不属于驱动器标签（“C:\”）的冒号字符 (:)。 |
| ArgumentException | path 是零长度字符串，仅包含空格，或者包含一个或多个无效字符。您可以使用 System.IO.Path.GetInvalidPathChars 方法查询无效字符。 - 或 - 路径仅以冒号字符 (:) 为前缀或仅包含冒号字符 (:)。 |
| IOException | path 指定的目录是一个文件。 - 或 - 网络名称未知。 |

### 评论

如果该目录不存在，将创建它。

### 例子

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 也可以看看

* class [CabArchive](../)
* 命名空间 [Aspose.Zip.Cab](../../cabarchive/)
* 部件 [Aspose.Zip](../../../)


