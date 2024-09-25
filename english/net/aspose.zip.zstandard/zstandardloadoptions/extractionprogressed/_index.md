---
title: ZstandardLoadOptions.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ZstandardLoadOptions event. Gets or sets the delegate invoked when some bytes have been extracted
type: docs
weight: 20
url: /net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Gets or sets the delegate invoked when some bytes have been extracted.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is the [`ZstandardArchive`](../../zstandardarchive/) instance which extraction is progressed.

## Examples

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


