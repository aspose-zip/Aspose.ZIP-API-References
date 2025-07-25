---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchiveEntry event. Raises when a portion of raw stream compressed
type: docs
weight: 70
url: /net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarks

Event sender is an [`SevenZipArchiveEntry`](../) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

## Examples

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


