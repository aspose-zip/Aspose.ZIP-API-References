---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: LzmaCompressionSettings constructor. Initializes a new instance of the LzmaCompressionSettings class with default parameters
type: docs
weight: 10
url: /net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings() {#constructor}

Initializes a new instance of the [`LzmaCompressionSettings`](../) class with default parameters.

```csharp
public LzmaCompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int, int, int) {#constructor_2}

Initializes a new instance of the [`LzmaCompressionSettings`](../) class with specified dictionary size, number of fast bytes and number of literal context bits.

```csharp
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | Int32 | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | Int32 | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### See Also

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int) {#constructor_1}

Initializes a new instance of the [`LzmaCompressionSettings`](../) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

```csharp
public LzmaCompressionSettings(int dictionarySize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | Int32 | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### See Also

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


