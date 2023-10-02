---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: RarArchiveEntry event. Raises when a portion of raw stream extracted
type: docs
weight: 80
url: /net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Raises when a portion of raw stream extracted.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is an [`RarArchiveEntry`](../) instance.

## Examples

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


