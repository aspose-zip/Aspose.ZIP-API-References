---
title: SharArchive.Save
second_title: Aspose.ZIP for .NET API 参考
description: SharArchive 方法. 将存档保存到提供的目标文件
type: docs
weight: 70
url: /zh/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

将存档保存到提供的目标文件。

```csharp
public void Save(string destinationFileName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的存档的路径。如果指定的文件名指向一个现有文件，它将被覆盖。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *destinationFileName*是零长度字符串，仅包含空格，或包含一个或多个由 System.IO.Path.InvalidPathChars 定义的无效字符。 |
| ArgumentNullException | *destinationFileName*一片空白。 |
| PathTooLongException | 指定的*destinationFileName*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| DirectoryNotFoundException | 指定的*destinationFileName*无效，（例如，它位于未映射的驱动器上）。 |
| IOException | 打开文件时发生 I/O 错误。 |
| UnauthorizedAccessException | *destinationFileName*指定了一个只读文件并且访问权限不是读取的。- 或 - 路径指定了一个目录。- 或 - 调用者没有所需的权限。 |
| NotSupportedException | *destinationFileName*格式无效。 |

### 评论

可以将存档保存到与从中加载的路径相同的路径。 但是，不建议这样做，因为这种方法使用复制到临时文件。

### 例子

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### 也可以看看

* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

将存档保存到提供的流中。

```csharp
public void Save(Stream output)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| output | Stream | 目标流。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *output*一片空白。 |
| ArgumentException | *output*不可写。 - 或者 -*output*是我们从中提取的同一个流。 |

### 评论

*output*必须是可写的。

### 例子

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### 也可以看看

* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)


