---
title: ZArchiveLoadOptions.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ZArchiveLoadOptions event. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 20
url: /net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is the [`ZArchive`](../../zarchive/) instance which extraction is progressed.

## Examples

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


