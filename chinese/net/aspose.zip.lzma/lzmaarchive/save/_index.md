---
title: LzmaArchive.Save
second_title: Aspose.ZIP for .NET API 参考
description: LzmaArchive 方法. 将 lzma 存档保存到提供的流中
type: docs
weight: 40
url: /zh/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

将 lzma 存档保存到提供的流中。

```csharp
public void Save(Stream output)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| output | Stream | 目标流。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *output*不支持寻找。 |
| ArgumentNullException | *output*一片空白。 |

### 评论

*output*必须是可寻的。

### 例子

```csharp
using (FileStream lzmaFile = File.Open("archive.lzma", FileMode.Create))
{
    using (var archive = new LzmaArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzmaFile);
     }
}
```

### 也可以看看

* class [LzmaArchive](../)
* 命名空间 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 部件 [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

将 lzma 存档保存到提供的目标文件中。

```csharp
public void Save(FileInfo destination)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destination | FileInfo | 将作为目标流打开的 FileInfo。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| SecurityException | 调用者没有所需的权限来打开*destination*. |
| ArgumentException | 文件路径为空或仅包含空格。 |
| FileNotFoundException | 找不到该文件。 |
| UnauthorizedAccessException | 文件路径是只读的或者是一个目录。 |
| ArgumentNullException | *destination*一片空白。 |
| DirectoryNotFoundException | 指定的路径无效，例如在未映射的驱动器上。 |
| IOException | 该文件已经打开。 |

### 例子

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### 也可以看看

* class [LzmaArchive](../)
* 命名空间 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 部件 [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

将 lzma 存档保存到提供的目标文件中。

```csharp
public void Save(string destinationFileName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的存档的路径。如果指定的文件名指向一个现有文件，它将被覆盖。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *destinationFileName*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*destinationFileName*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*destinationFileName*被拒绝。 |
| PathTooLongException | 指定的*destinationFileName*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*destinationFileName*在字符串中间包含一个冒号 (:)。 |

### 例子

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### 也可以看看

* class [LzmaArchive](../)
* 命名空间 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 部件 [Aspose.Zip](../../../)


