---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ArchiveFactory 方法。使用提供的归档格式将指定目录压缩为归档文件"
type: docs
weight: 10
url: /zh/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

使用提供的归档格式将指定目录压缩为归档文件。

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 将被压缩的目录路径。 |
| outputFileName | String | 目标文件名。 |
| archiveFormat | ArchiveFormat | 要创建的归档格式（例如 zip、rar、tar 等）。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| DirectoryNotFoundException | 如果 *path* 指定的目录不存在，则抛出此异常。 |
| ArgumentException | 如果 *path* 为 null 或空字符串，则抛出此异常。 |
| NotSupportedException | 如果指定的 *archiveFormat* 不受支持或无法识别，则抛出此异常。 |
| ArgumentNullException | *path* 为 `null`。 |

## 备注

此方法将在 *path* 参数指定的位置创建归档文件。归档文件的名称通常为目录名称，后跟基于 *archiveFormat* 的相应文件扩展名。目录本身不会被修改或删除。

## 示例

以下是如何使用 CompressDirectory 方法的示例：

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// 这将在指定路径下创建一个包含该目录内容的 ZIP 文件。
```

### 另请参阅

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


