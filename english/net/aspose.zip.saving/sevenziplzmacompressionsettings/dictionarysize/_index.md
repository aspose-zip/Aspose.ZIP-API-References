---
title: SevenZipLZMACompressionSettings.DictionarySize
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipLZMACompressionSettings property. Dictionary history buffer size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set will be chosen accordingly to entry size
type: docs
weight: 20
url: /net/aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/
---
## SevenZipLZMACompressionSettings.DictionarySize property

Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size.

```csharp
public int DictionarySize { get; set; }
```

## Remarks

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

### See Also

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


