---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LhaArchiveEntry 方法。按路径将 Lha 存档条目提取到文件系统。"
type: docs
weight: 60
url: /zh/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

按路径将 Lha 存档条目提取到文件系统。

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
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

## 示例

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 另请参阅

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

## 备注

对目录条目不执行任何操作。

### 另请参阅

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

将 Lha 存档条目提取到文件。

```csharp
public void Extract(FileInfo fileInfo)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileInfo | FileInfo | 用于存储解压缩数据的 FileInfo。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 未读取存档头部和服务信息。 |
| SecurityException | 调用者没有打开 *fileInfo* 所需的权限。 |
| ArgumentException | 文件路径为空或仅包含空白字符。 |
| FileNotFoundException | 未找到该文件。 |
| UnauthorizedAccessException | 文件路径为只读或是目录。 |
| ArgumentNullException | *fileInfo* 为 null。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |

## 备注

对目录条目不执行任何操作。

## 示例

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 另请参阅

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


