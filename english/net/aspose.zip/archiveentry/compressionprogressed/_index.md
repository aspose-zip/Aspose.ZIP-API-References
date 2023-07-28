---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveEntry event. Raises when a portion of raw stream compressed
type: docs
weight: 80
url: /net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarks

Event sender is an [`ArchiveEntry`](../) instance.

## Examples

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


