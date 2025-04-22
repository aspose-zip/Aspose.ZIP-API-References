---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipLZMA2CompressionSettings constructor. Instantiates settings for LZMA2 compression method within 7z archive
type: docs
weight: 10
url: /net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instantiates settings for LZMA2 compression method within 7z archive.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | The Size of history buffer, must be between 4096 and 1073741824. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* is too big or too small. |

## Remarks

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

### See Also

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instantiates settings for LZMA2 compression method within 7z archive.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | The size of history buffer, must be between 4096 and 1073741824. |
| fastBytes | Int32 | Controls the number of fast bytes used by the LZMA2 compressors. A larger number of fast bytes can provide a better compression ratio at the expense of compression speed. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* is too big or too small, or *fastBytes* is too big or too small. |

## Remarks

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

### See Also

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


