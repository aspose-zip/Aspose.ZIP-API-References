---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LzxArchiveEntry 方法。将 Lzx 存档条目提取到文件系统的指定路径"
type: docs
weight: 80
url: /zh/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

按路径将 Lzx 存档条目提取到文件系统。

```csharp
public FileSystemInfo Extract(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 用于存储解压后数据的文件路径。 |

### Return Value

包含已提取数据的 FileSystemInfoInstance。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 未读取存档头部和服务信息。 |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| InvalidDataException | 标题或数据的校验和不匹配。- 或 - 归档已损坏。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| NotSupportedException | 无效的压缩方法。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |

## 示例

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 另请参阅

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

将条目提取到提供的流中。

```csharp
public void Extract(Stream destination)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | 流 | 目标流。必须可写。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | *destination* 不支持写入。 |
| InvalidDataException | 标题或数据的校验和不匹配。- 或 - 归档已损坏。 |
| ArgumentNullException | 目标流为 null。 |
| NotSupportedException | 无效的压缩方法。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |

### 另请参阅

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


