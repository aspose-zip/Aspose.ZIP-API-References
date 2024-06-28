---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveEntry event. Raises when a portion of raw stream extracted
type: docs
weight: 90
url: /net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Raises when a portion of raw stream extracted.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is an [`ArchiveEntry`](../) instance.

## Examples

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### See Also

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


