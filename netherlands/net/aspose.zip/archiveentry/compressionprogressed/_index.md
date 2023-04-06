---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveEntry evenement. Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd.
type: docs
weight: 80
url: /nl/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Opmerkingen

Afzender van gebeurtenis is een[`ArchiveEntry`](../) voorbeeld.

### Voorbeelden

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* naamruimte [Aspose.Zip](../../archiveentry/)
* montage [Aspose.Zip](../../../)


