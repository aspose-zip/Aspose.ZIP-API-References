---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP voor .NET API-referentie
description: RarArchiveEntry evenement. Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd.
type: docs
weight: 80
url: /nl/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Opmerkingen

Afzender van gebeurtenis is een[`RarArchiveEntry`](../) voorbeeld.

### Voorbeelden

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* naamruimte [Aspose.Zip.Rar](../../rararchiveentry/)
* montage [Aspose.Zip](../../../)


