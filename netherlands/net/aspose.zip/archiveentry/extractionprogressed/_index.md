---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveEntry evenement. Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd.
type: docs
weight: 90
url: /nl/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Opmerkingen

Afzender van gebeurtenis is een[`ArchiveEntry`](../) voorbeeld.

### Voorbeelden

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Zie ook

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* naamruimte [Aspose.Zip](../../archiveentry/)
* montage [Aspose.Zip](../../../)


