---
title: Bzip2LoadOptions.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2LoadOptions event. Event raised invoked when some bytes have been extracted
type: docs
weight: 20
url: /net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Event raised invoked when some bytes have been extracted.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarks

Event sender is the [`Bzip2Archive`](../../bzip2archive/) instance which extraction is progressed. The [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) is the number of bytes after extraction.

## Examples

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


