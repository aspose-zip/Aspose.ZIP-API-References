---
title: Class SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Saving.SevenZipLZMA2CompressionSettings class. Settings for LZMA2 compression method within 7z archive
type: docs
weight: 810
url: /net/aspose.zip.saving/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings class

Settings for LZMA2 compression method within 7z archive.

```csharp
public class SevenZipLZMA2CompressionSettings : SevenZipCompressionSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor)(int) | Instantiates settings for LZMA2 compression method within 7z archive. |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor_1)(int, int) | Instantiates settings for LZMA2 compression method within 7z archive. |

## Properties

| Name | Description |
| --- | --- |
| [CompressionThreads](../../aspose.zip.saving/sevenziplzma2compressionsettings/compressionthreads/) { get; set; } | Gets or sets compression thread count. If the value is greater than 1, multithreading compression will be used. |
| [DictionarySize](../../aspose.zip.saving/sevenziplzma2compressionsettings/dictionarysize/) { get; } | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. |
| [FastBytes](../../aspose.zip.saving/sevenziplzma2compressionsettings/fastbytes/) { get; } | Gets the control number of fast bytes used by the LZMA2 compressor. |
| override [Method](../../aspose.zip.saving/sevenziplzma2compressionsettings/method/) { get; } | Gets compression or decompression method. |

## Remarks

LZMA2 supports multiple runs of compressed LZMA data and uncompressed data.

See more: https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm

### See Also

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


