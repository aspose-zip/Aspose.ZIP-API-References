---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveEntry händelse. Ökar när en del av råström extraheras.
type: docs
weight: 90
url: /sv/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Ökar när en del av råström extraheras.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Anmärkningar

Händelseavsändaren är en[`ArchiveEntry`](../) exempel.

### Exempel

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Se även

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namnutrymme [Aspose.Zip](../../archiveentry/)
* hopsättning [Aspose.Zip](../../../)


