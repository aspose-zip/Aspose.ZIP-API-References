---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveLoadOptions property. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 50
url: /net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public EventHandler<ProgressCancelEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarks

Event sender is the [`ArchiveEntry`](../../archiveentry/) instance which extraction is progressed.

## Examples

Track the progress of an entry extraction.

```csharp
var archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

Cancel an entry extraction after a certain time.

```csharp
Stopwatch watch = Stopwatch.StartNew();
using (Archive a = new Archive("big.zip", new ArchiveLoadOptions() {
    EntryExtractionProgressed = (s, e) => { if (watch.ElapsedMilliseconds > 1000) e.Cancel = true; } }))
{
    a.Entries[0].Extract("first.bin");
}
```

### See Also

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


