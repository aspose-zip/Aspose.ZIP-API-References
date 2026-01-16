---
title: Class SevenZipLZMACompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Saving.SevenZipLZMACompressionSettings class. Settings for LZMA compression method within 7z archive
type: docs
weight: 880
url: /net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Settings for LZMA compression method within 7z archive.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor)() | Initializes a new instance of the `SevenZipLZMACompressionSettings` class with default parameters. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_1)(int) | Initializes a new instance of the `SevenZipLZMACompressionSettings` class with specified dictionary size, number of fast bytes equal to 32, number of literal context bits equal to 3. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_2)(int, int, int) | Initializes a new instance of the `SevenZipLZMACompressionSettings` class with specified dictionary size, number of fast bytes and number of literal context bits. |

## Properties

| Name | Description |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |
| [LiteralContextBits](../../aspose.zip.saving/sevenziplzmacompressionsettings/literalcontextbits/) { get; } | Gets the number of literal context bits. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Gets compression or decompression method. |
| [NumberOfFastBytes](../../aspose.zip.saving/sevenziplzmacompressionsettings/numberoffastbytes/) { get; } | Gets the number of bytes used for fast match searching in the LZMA algorithm. |

## Remarks

The Lempel–Ziv–Markov chain algorithm (LZMA) is an algorithm used to perform lossless data compression. This algorithm uses a dictionary compression scheme somewhat similar to the LZ77 algorithm and features a high compression ratio and a variable compression-dictionary size.

See more: [Lempel–Ziv–Markov chain algorithm](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### See Also

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


