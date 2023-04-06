---
title: ZArchive.Extract
second_title: Aspose.ZIP for .NET API 参考
description: ZArchive 方法. 将 Z 存档提取到流中
type: docs
weight: 30
url: /zh/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

将 Z 存档提取到流中。

```csharp
public void Extract(Stream destination)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destination | Stream | 用于存储解压缩数据的流。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidDataException | 数据无法解压。 |

### 例子

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

将 Z 存档提取到文件中。

```csharp
public void Extract(FileInfo fileInfo)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo 用于存储解压后的数据。 |

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
| InvalidDataException | 数据无法解压。 |

### 例子

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

通过路径将 Z 存档提取到文件。

```csharp
public FileInfo Extract(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 将存储解压缩数据的文件的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |
| InvalidDataException | 数据无法解压。 |

### 例子

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)


