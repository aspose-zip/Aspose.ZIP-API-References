---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveLoadOptions fast egendom. Hämtar eller ställer in ombudet som anropas när några byte har extraherats.
type: docs
weight: 40
url: /sv/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Hämtar eller ställer in ombudet som anropas när några byte har extraherats.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Anmärkningar

Händelsens avsändare är[`ArchiveEntry`](../../archiveentry/) exempel vilken utvinning fortskrider.

### Exempel

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Se även

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* namnutrymme [Aspose.Zip](../../archiveloadoptions/)
* hopsättning [Aspose.Zip](../../../)


