---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZstandardSaveOptions gebeurtenis. Wordt geactiveerd wanneer een deel van de ruwe stroom is gecomprimeerd."
type: docs
weight: 20
url: /nl/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Wordt opgegooid wanneer een deel van de ruwe stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Voorbeelden

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


