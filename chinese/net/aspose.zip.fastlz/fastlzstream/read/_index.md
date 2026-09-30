---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP for .NET API 参考"
description: "FastLZStream 方法。从流中读取一系列字节，并根据读取的字节数前进流中的位置。不支持"
type: docs
weight: 90
url: /zh/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

从流中读取一系列字节，并将流中的位置前移读取的字节数。不支持。

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 缓冲区 | Byte[] | 字节数组。当此方法返回时，buffer 包含指定的字节数组，其中 offset 到 (offset + count - 1) 之间的值已被从当前源读取的字节替换。 |
| 偏移量 | Int32 | 在 buffer 中的基于零的字节偏移量，从该位置开始存储从当前流读取的数据。 |
| count | Int32 | 从当前流读取的最大字节数。 |

### Return Value

读取到 buffer 中的字节总数。如果当前可用字节不足请求的字节数，则可能少于请求的字节数；如果已到达流的末尾，则为零 (0)。

### 异常

| 异常 | 条件 |
| --- | --- |
| NotSupportedException | 此操作不受支持。 |

### 另请参阅

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


