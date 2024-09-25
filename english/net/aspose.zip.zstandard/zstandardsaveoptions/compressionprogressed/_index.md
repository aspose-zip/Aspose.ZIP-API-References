---
title: ZstandardSaveOptions.CompressionProgressed
second_title: Aspose.ZIP for .NET API Reference
description: ZstandardSaveOptions event. Raises when a portion of raw stream compressed
type: docs
weight: 20
url: /net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Raises when a portion of raw stream compressed.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Examples

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### See Also

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


