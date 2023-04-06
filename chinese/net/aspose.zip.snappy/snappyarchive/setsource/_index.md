---
title: SnappyArchive.SetSource
second_title: Aspose.ZIP for .NET API 参考
description: SnappyArchive 方法. 设置要在存档中压缩的内容
type: docs
weight: 50
url: /zh/net/aspose.zip.snappy/snappyarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

设置要在存档中压缩的内容。

```csharp
public void SetSource(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的输入流。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | 这*source*流是不可搜索的。 |

### 例子

```csharp
using (var archive = new SnappyArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.snappy");
}
```

### 也可以看看

* class [SnappyArchive](../)
* 命名空间 [Aspose.Zip.Snappy](../../snappyarchive/)
* 部件 [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

设置要在存档中压缩的内容。

```csharp
public void SetSource(FileInfo fileInfo)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileInfo | FileInfo | 将作为输入流打开的 FileInfo。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| SecurityException | 调用者没有所需的权限来打开*fileInfo*. |
| ArgumentException | 文件路径为空或仅包含空格。 |
| FileNotFoundException | 找不到该文件。 |
| UnauthorizedAccessException | 文件路径是只读的或者是一个目录。 |
| ArgumentNullException | *fileInfo*一片空白。 |
| DirectoryNotFoundException | 指定的路径无效，例如在未映射的驱动器上。 |
| IOException | 该文件已经打开。 |

### 例子

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.snappy");
}
```

### 也可以看看

* class [SnappyArchive](../)
* 命名空间 [Aspose.Zip.Snappy](../../snappyarchive/)
* 部件 [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

设置要在存档中压缩的内容。

```csharp
public void SetSource(string sourcePath)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourcePath | String | 将作为输入流打开的文件的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *sourcePath*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*sourcePath*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*sourcePath*被拒绝。 |
| PathTooLongException | 指定的*sourcePath*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*sourcePath*在字符串中间包含一个冒号 (:)。 |

### 例子

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### 也可以看看

* class [SnappyArchive](../)
* 命名空间 [Aspose.Zip.Snappy](../../snappyarchive/)
* 部件 [Aspose.Zip](../../../)


