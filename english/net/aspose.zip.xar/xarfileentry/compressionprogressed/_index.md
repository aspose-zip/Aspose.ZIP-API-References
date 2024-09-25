---
title: XarFileEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: XarFileEntry event. Raises when a portion of raw stream compressed
type: docs
weight: 20
url: /net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarks

Event sender is an [`XarFileEntry`](../) instance.

## Examples

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


