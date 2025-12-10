---
title: Class LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Saving.LzmaCompressionSettings class. Settings for LZMA compression within a ZIP archive
type: docs
weight: 750
url: /net/aspose.zip.saving/lzmacompressionsettings/
---
## LzmaCompressionSettings class

Settings for LZMA compression within a ZIP archive.

```csharp
public class LzmaCompressionSettings : CompressionSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor)() | Initializes a new instance of the `LzmaCompressionSettings` class with default parameters. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_1)(int) | Initializes a new instance of the `LzmaCompressionSettings` class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_2)(int, int, int) | Initializes a new instance of the `LzmaCompressionSettings` class with specified dictionary size, number of fast bytes and number of literal context bits. |

## Properties

| Name | Description |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/lzmacompressionsettings/dictionarysize/) { get; } | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. |
| [LiteralContextBits](../../aspose.zip.saving/lzmacompressionsettings/literalcontextbits/) { get; } | Gets the number of literal context bits. |
| [NumberOfFastBytes](../../aspose.zip.saving/lzmacompressionsettings/numberoffastbytes/) { get; } | Gets the number of bytes used for fast match searching in the LZMA algorithm. |

## Remarks

The Lempel–Ziv–Markov chain algorithm (LZMA) is an algorithm used to perform lossless data compression. This algorithm uses a dictionary compression scheme somewhat similar to the LZ77 algorithm and features a high compression ratio and a variable compression-dictionary size.

See more: [Lempel–Ziv–Markov chain algorithm](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### See Also

* class [CompressionSettings](../compressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


