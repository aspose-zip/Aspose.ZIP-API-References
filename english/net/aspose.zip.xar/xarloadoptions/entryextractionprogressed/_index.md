---
title: XarLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: XarLoadOptions property. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 20
url: /net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarks

Event sender is the [`XarFileEntry`](../../xarfileentry/) instance which extraction is progressed.

## Examples

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


