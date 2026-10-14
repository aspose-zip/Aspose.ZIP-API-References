---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchiveEntry 方法。根据提供的路径将条目提取到文件系统"
type: docs
weight: 50
url: /zh/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

按提供的路径将条目提取到文件系统中。

```csharp
public FileInfo Extract(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 目标文件的路径。如果文件已存在，将被覆盖。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidDataException | 条目存储的校验和或摘要与提取的数据不匹配。 |
| InvalidOperationException | 该条目属于为组合准备的归档，或无法从不可定位的归档流中打开条目数据。 |
| NotSupportedException | 该条目属于固体 Apple Archive，或使用了不受支持的压缩方法。 |
| ObjectDisposedException | 源流已被释放。 |
| IOException | 发生 I/O 错误。 |

### 另请参阅

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
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
| ArgumentNullException | *destination* 为 `null`。 |
| ArgumentException | *destination* 不支持写入。 |
| InvalidDataException | 条目存储的校验和或摘要与提取的数据不匹配。 |
| InvalidOperationException | 该条目属于为组合准备的归档，或无法从不可定位的归档流中打开条目数据。 |
| NotSupportedException | 该条目属于固体 Apple Archive，或使用了不受支持的压缩方法。 |
| ObjectDisposedException | 源流已被释放。 |
| IOException | 发生 I/O 错误。 |

### 另请参阅

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


