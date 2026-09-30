---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzmaArchiveSettings Ereignis. Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird."
type: docs
weight: 50
url: /de/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Beispiele

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


