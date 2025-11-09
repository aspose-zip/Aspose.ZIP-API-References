---
title: SevenZipLZMACompressionSettings.SevenZipLZMACompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipLZMACompressionSettings constructor. Initializes a new instance of the SevenZipLZMACompressionSettings class with default parameters
type: docs
weight: 10
url: /net/aspose.zip.saving/sevenziplzmacompressionsettings/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings() {#constructor}

Initializes a new instance of the [`SevenZipLZMACompressionSettings`](../) class with default parameters.

```csharp
public SevenZipLZMACompressionSettings()
```

## Examples

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save("result.7z");
}
```

### See Also

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int, int, int) {#constructor_2}

Initializes a new instance of the [`SevenZipLZMACompressionSettings`](../) class with specified dictionary size, number of fast bytes and number of literal context bits.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, 
    int literalContextBits)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |
| numberOfFastBytes | Int32 | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | Int32 | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### See Also

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int) {#constructor_1}

Initializes a new instance of the [`SevenZipLZMACompressionSettings`](../) class with specified dictionary size, number of fast bytes equal to 32, number of literal context bits equal to 3.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |

### See Also

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


