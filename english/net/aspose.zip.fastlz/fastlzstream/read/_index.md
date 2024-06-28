---
title: FastLZStream.Read
second_title: Aspose.ZIP for .NET API Reference
description: FastLZStream method. Reads a sequence of bytes from the stream and advances the position within the stream by the number of bytes read. Not supported
type: docs
weight: 90
url: /net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Reads a sequence of bytes from the stream and advances the position within the stream by the number of bytes read. Not supported.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parameter | Type | Description |
| --- | --- | --- |
| buffer | Byte[] | An array of bytes. When this method returns, the buffer contains the specified byte array with the values between offset and (offset + count - 1) replaced by the bytes read from the current source. |
| offset | Int32 | The zero-based byte offset in buffer at which to begin storing the data read from the current stream. |
| count | Int32 | The maximum number of bytes to be read from the current stream. |

### Return Value

The total number of bytes read into the buffer. This can be less than the number of bytes requested if that many bytes are not currently available, or zero (0) if the end of the stream has been reached.

### See Also

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


