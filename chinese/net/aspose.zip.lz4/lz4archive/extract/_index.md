---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Lz4Archive 方法。将归档按路径提取到文件。"
type: docs
weight: 30
url: /zh/net/aspose.zip.lz4/lz4archive/extract/
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
| EndOfStreamException | 源流太短。 |
| InvalidDataException | 解码时发现错误的字节。 |
| NotSupportedException | 不支持此 LZ4 版本。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 已准备好进行组合的归档。 |

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

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
| ArgumentException | *destination* 不支持写入。 |
| EndOfStreamException | 源流太短。 |
| InvalidDataException | 解码时发现错误的字节。 |
| NotSupportedException | 不支持此 LZ4 版本。 |
| InvalidOperationException | 已准备好进行组合的归档。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


