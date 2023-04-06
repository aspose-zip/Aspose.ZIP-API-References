---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchiveEntry evenement. Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd.
type: docs
weight: 70
url: /nl/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Opmerkingen

Afzender van gebeurtenis is een[`SevenZipArchiveEntry`](../) voorbeeld.

### Voorbeelden

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* montage [Aspose.Zip](../../../)


