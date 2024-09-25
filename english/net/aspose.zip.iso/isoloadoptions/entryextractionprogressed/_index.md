---
title: IsoLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: IsoLoadOptions property. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 20
url: /net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarks

Event sender is the [`IsoEntry`](../../isoentry/) instance which extraction is progressed.

## Examples

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


