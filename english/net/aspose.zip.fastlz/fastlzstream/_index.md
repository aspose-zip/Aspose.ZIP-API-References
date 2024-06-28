---
title: Class FastLZStream
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.FastLZ.FastLZStream class. A stream wrapper that compresses data with FastLZ. Implements decorator pattern
type: docs
weight: 210
url: /net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

A stream wrapper that compresses data with FastLZ. Implements decorator pattern.

```csharp
public class FastLZStream : Stream
```

## Constructors

| Name | Description |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Initializes a new instance of the `FastLZStream` class prepared for compression. |

## Properties

| Name | Description |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Gets a value indicating whether the current stream supports reading. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Gets a value indicating whether the current stream supports seeking. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Gets a value indicating whether the current stream supports writing. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Gets the length in bytes of the stream. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Gets or sets the position within the current stream. |

## Methods

| Name | Description |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Closes the current stream and releases any resources (such as sockets and file handles) associated with the current stream. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Clears all buffers for this stream and causes any buffered data to be written to the underlying device. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Reads a sequence of bytes from the stream and advances the position within the stream by the number of bytes read. Not supported. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Sets the position within the current stream. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Sets the length of the current stream. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Writes a sequence of bytes to the compressing stream and advances the current position within this stream by the number of bytes written. |

### See Also

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


