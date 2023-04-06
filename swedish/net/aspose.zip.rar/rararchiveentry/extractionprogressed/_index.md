---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: RarArchiveEntry händelse. Ökar när en del av råström extraheras.
type: docs
weight: 80
url: /sv/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Ökar när en del av råström extraheras.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Anmärkningar

Händelseavsändaren är en[`RarArchiveEntry`](../) exempel.

### Exempel

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namnutrymme [Aspose.Zip.Rar](../../rararchiveentry/)
* hopsättning [Aspose.Zip](../../../)


