---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchiveEntry 方法。打开条目以进行提取，并提供包含条目内容的流"
type: docs
weight: 60
url: /zh/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

打开条目以进行提取，并提供包含条目内容的流。

```csharp
public Stream Open()
```

### Return Value

一个可读取的流，包含提取的条目数据。

### 异常

| 异常 | 条件 |
| --- | --- |
| NotSupportedException | 该条目属于固体 Apple Archive，或使用了不受支持的压缩方法。 |
| InvalidDataException | 条目存储的校验和或摘要与提取的数据不匹配。 |
| InvalidOperationException | 该条目属于为组合准备的归档，或无法从不可定位的归档流中打开条目数据。 |
| ObjectDisposedException | 源流已被释放。 |
| IOException | 发生 I/O 错误。 |

## 备注

从返回的流中读取以获取原始条目内容。如果归档包含校验和字段，则在读取返回的流时会验证校验和。

### 另请参阅

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


