---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveLoadOptions eigendom. Haalt of stelt de gemachtigde in die wordt aangeroepen wanneer een item wordt vermeld in de inhoudsopgave.
type: docs
weight: 50
url: /nl/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Haalt of stelt de gemachtigde in die wordt aangeroepen wanneer een item wordt vermeld in de inhoudsopgave.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Voorbeelden

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Zie ook

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* naamruimte [Aspose.Zip](../../archiveloadoptions/)
* montage [Aspose.Zip](../../../)


