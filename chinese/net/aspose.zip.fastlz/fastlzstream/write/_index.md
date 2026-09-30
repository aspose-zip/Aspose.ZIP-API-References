---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP for .NET API 参考"
description: "FastLZStream 方法。将一系列字节写入压缩流，并根据写入的字节数前进此流中的当前位置"
type: docs
weight: 120
url: /zh/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

将一系列字节写入压缩流，并将此流中的当前位置前移写入的字节数。

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 缓冲区 | Byte[] | 字节数组。此方法将 count 字节从 buffer 复制到当前流。 |
| 偏移量 | Int32 | 在 buffer 中的基于零的字节偏移量，从该位置开始将字节复制到当前流。 |
| count | Int32 | 要写入当前流的字节数。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 如果流已被释放，则抛出此异常。 |
| ArgumentNullException | *buffer* 为 `null`。 |

### 另请参阅

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


