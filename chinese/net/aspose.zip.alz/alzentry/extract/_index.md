---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AlzEntry 方法。根据提供的路径将条目提取到文件系统中"
type: docs
weight: 60
url: /zh/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

按提供的路径将条目提取到文件系统中。

```csharp
public FileInfo Extract(string path, string password = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 目标文件的路径。如果文件已存在，将被覆盖。 |
| 密码 | String | 用于解密的可选密码。 |

### Return Value

复合文件的文件信息。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| InvalidDataException | 存档已损坏。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| FileNotFoundException | 未找到该文件。 |

## 示例

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### 另请参阅

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

将条目提取到提供的流中。

```csharp
public void Extract(Stream destination, string password = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | 流 | 目标流。必须可写。 |
| 密码 | String | 用于解密的可选密码。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | *destination* 不支持写入。 |
| InvalidOperationException | 存档未打开以进行提取。- 或 - 此条目是目录。 |
| InvalidDataException | 条目中的数据错误。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |

## 示例

使用密码提取 ALZ 存档的条目。

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### 另请参阅

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


