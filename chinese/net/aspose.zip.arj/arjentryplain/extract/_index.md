---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ArjEntryPlain 方法。根据提供的路径将条目提取到文件系统"
type: docs
weight: 40
url: /zh/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

按提供的路径将条目提取到文件系统中。

```csharp
public FileInfo Extract(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 目标文件的路径。如果文件已存在，将被覆盖。 |

### Return Value

复合文件的文件信息。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null 或为空。 |
| ObjectDisposedException | 如果存档已被释放，则抛出此异常。 |
| FileNotFoundException | 未找到该文件。 |
| InvalidDataException | 标题或数据的校验和不匹配。- 或 - 归档已损坏。 |
| PathTooLongException | 指定的路径、文件名或两者的长度超过系统定义的最大长度。 |
| NotImplementedException | 使用方法 4 压缩的条目。 |

## 示例

提取 rar 存档的两个条目。

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### 另请参阅

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

将 ARJ 存档条目提取到文件。

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
| ObjectDisposedException | 如果存档已被释放，则抛出此异常。 |
| InvalidDataException | 标题或数据的校验和不匹配。- 或 - 归档已损坏。 |
| NotImplementedException | 使用方法 4 压缩的条目。 |

## 示例

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 另请参阅

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | 标题或数据的校验和不匹配。- 或 - 归档已损坏。 |
| NotImplementedException | 使用方法 4 压缩的条目。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 如果存档已被释放，则抛出此异常。 |

### 另请参阅

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


