---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveLoadOptions eigendom. Haalt of stelt de gemachtigde in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.
type: docs
weight: 40
url: /nl/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Haalt of stelt de gemachtigde in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Opmerkingen

Gebeurtenisafzender is de[`ArchiveEntry`](../../archiveentry/) instantie welke extractie wordt uitgevoerd.

### Voorbeelden

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Zie ook

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* naamruimte [Aspose.Zip](../../archiveloadoptions/)
* montage [Aspose.Zip](../../../)


