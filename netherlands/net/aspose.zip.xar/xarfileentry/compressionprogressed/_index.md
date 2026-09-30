---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarFileEntry event. Wordt opgewekt wanneer een deel van de ruwe stroom is gecomprimeerd"
type: docs
weight: 20
url: /nl/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Wordt opgegooid wanneer een deel van de ruwe stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Opmerkingen

Eventzender is een [`XarFileEntry`](../) instantie.

## Voorbeelden

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


