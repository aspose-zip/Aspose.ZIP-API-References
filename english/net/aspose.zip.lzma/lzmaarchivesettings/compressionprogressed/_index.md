---
title: LzmaArchiveSettings.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: LzmaArchiveSettings event. Raises when a portion of raw stream compressed
type: docs
weight: 50
url: /net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Examples

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


