---
title: "UueArchive.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "UueArchive 方法。将存档提取到提供的流中"
type: docs
weight: 40
url: /zh/net/aspose.zip.uue/uuearchive/extract/
---
## Extract(Stream) {#extract_1}

将存档提取到提供的流中。

```csharp
public void Extract(Stream destination)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | 流 | 目标流。必须可写。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentException | *destination* 不支持写入。 |

## 示例

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

将存档提取到指定路径的文件中。

```csharp
public FileInfo Extract(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 目标文件的路径。如果文件已存在，将被覆盖。 |

### Return Value

已提取文件的信息。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| FileNotFoundException | 未找到该文件。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


