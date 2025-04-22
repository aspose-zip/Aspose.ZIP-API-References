---
title: LzmaArchiveSettings.DictionarySize
second_title: Aspose.ZIP for .NET API Reference
description: LzmaArchiveSettings property. Dictionary history buffer size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set will be chosen accordingly to entry size
type: docs
weight: 20
url: /net/aspose.zip.lzma/lzmaarchivesettings/dictionarysize/
---
## LzmaArchiveSettings.DictionarySize property

Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

```csharp
public int DictionarySize { get; set; }
```

## Remarks

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

### See Also

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


