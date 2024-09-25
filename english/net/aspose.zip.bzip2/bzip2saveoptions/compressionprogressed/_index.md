---
title: Bzip2SaveOptions.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2SaveOptions event. Raises when a portion of raw stream compressed
type: docs
weight: 40
url: /net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarks

This event won't be raised when compressing in multithreaded mode.

## Examples

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


