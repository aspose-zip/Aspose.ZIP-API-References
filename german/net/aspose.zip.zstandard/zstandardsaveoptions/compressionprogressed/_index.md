---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardSaveOptions-Ereignis. Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird."
type: docs
weight: 20
url: /de/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Beispiele

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


