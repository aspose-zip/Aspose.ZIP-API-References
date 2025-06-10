---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveEntry event. Raises when a portion of raw stream extracted
type: docs
weight: 100
url: /net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Raises when a portion of raw stream extracted.

```csharp
public event EventHandler<ProgressCancelEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is an [`ArchiveEntry`](../) instance. It is possible to cancel extraction.

## Examples

In this sample event handler is used for calculation the share of proceeded size in percents.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => { if (e.ProceededBytes > 100000000) e.Cancel = true; };
```

### See Also

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


