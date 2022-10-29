---
title: ExtractionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: Ökar när en del av råström extraheras.
type: docs
weight: 80
url: /sv/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Ökar när en del av råström extraheras.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Anmärkningar

Händelseavsändaren är en[`ArchiveEntry`](../../archiveentry) exempel.

### Exempel

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Se även

* class [ProgressEventArgs](../../progresseventargs)
* class [ArchiveEntry](../../archiveentry)
* namnutrymme [Aspose.Zip](../../archiveentry)
* hopsättning [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->