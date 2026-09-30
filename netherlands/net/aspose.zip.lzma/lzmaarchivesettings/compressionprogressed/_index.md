---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LzmaArchiveSettings event. Wordt opgewekt wanneer een deel van de ruwe stroom is gecomprimeerd"
type: docs
weight: 50
url: /nl/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Wordt opgegooid wanneer een deel van de ruwe stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Voorbeelden

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


