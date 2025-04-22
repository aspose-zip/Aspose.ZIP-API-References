---
title: FastLZStream.FastLZStream
second_title: Aspose.ZIP for .NET API Reference
description: FastLZStream constructor. Initializes a new instance of the FastLZStream class prepared for compression
type: docs
weight: 10
url: /net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Initializes a new instance of the [`FastLZStream`](../) class prepared for compression.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream for saving compressed data. |
| compressionLevel | Int32 | Use 1 for faster compression, use 2 for a better compression ratio. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* does not support writing. |
| ArgumentOutOfRangeException | *compressionLevel* is more than 2 or less than 1. |

### See Also

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


