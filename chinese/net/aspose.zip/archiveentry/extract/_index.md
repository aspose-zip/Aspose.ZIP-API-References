---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveEntry 方法. 通过提供的路径将条目提取到文件系统
type: docs
weight: 100
url: /zh/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

通过提供的路径将条目提取到文件系统。

```csharp
public FileInfo Extract(string path, string password = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 目标文件的路径。如果该文件已经存在，它将被覆盖。 |
| password | String | 用于解密的可选密码。 |

### 返回值

组合文件的文件信息。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |
| InvalidDataException | 条目的 CRC 或 MAC 验证失败。 |

### 例子

提取两个 zip 存档条目，每个条目都有自己的密码

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### 也可以看看

* class [ArchiveEntry](../)
* 命名空间 [Aspose.Zip](../../archiveentry/)
* 部件 [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

将条目提取到所提供的流中。

```csharp
public void Extract(Stream destination, string password = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destination | Stream | 目标流。必须是可写的。 |
| password | String | 用于解密的可选密码。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidDataException | 条目的 CRC 或 MAC 验证失败。 |
| ArgumentException | *destination*不支持写入。 |

### 例子

使用密码提取 zip 存档的条目。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### 也可以看看

* class [ArchiveEntry](../)
* 命名空间 [Aspose.Zip](../../archiveentry/)
* 部件 [Aspose.Zip](../../../)


