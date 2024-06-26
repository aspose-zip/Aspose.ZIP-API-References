---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveLoadOptions property. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 40
url: /net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarks

Event sender is the [`ArchiveEntry`](../../archiveentry/) instance which extraction is progressed.

## Examples

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### See Also

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


