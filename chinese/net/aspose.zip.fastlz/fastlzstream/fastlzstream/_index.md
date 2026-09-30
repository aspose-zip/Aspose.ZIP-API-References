---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP for .NET API 参考"
description: "FastLZStream 构造函数。初始化一个用于压缩的 FastLZStream 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

初始化一个用于压缩的 [`FastLZStream`](../) 类的新实例。

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于保存压缩数据的流。 |
| compressionLevel | Int32 | 使用 1 可获得更快的压缩，使用 2 可获得更好的压缩比。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* 为 null。 |
| ArgumentException | *stream* 不支持写入。 |
| ArgumentOutOfRangeException | *compressionLevel* 大于 2 或小于 1。 |

### 另请参阅

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


