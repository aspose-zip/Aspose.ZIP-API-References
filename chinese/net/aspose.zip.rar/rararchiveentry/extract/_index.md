---
title: RarArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API 参考
description: RarArchiveEntry 方法. 通过提供的路径将条目提取到文件系统
type: docs
weight: 90
url: /zh/net/aspose.zip.rar/rararchiveentry/extract/
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

提取 rar 存档的两个条目。

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### 也可以看看

* class [RarArchiveEntry](../)
* 命名空间 [Aspose.Zip.Rar](../../rararchiveentry/)
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

使用密码提取 rar 存档的条目。

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### 也可以看看

* class [RarArchiveEntry](../)
* 命名空间 [Aspose.Zip.Rar](../../rararchiveentry/)
* 部件 [Aspose.Zip](../../../)


