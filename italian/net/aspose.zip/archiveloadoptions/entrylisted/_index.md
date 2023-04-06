---
title: ArchiveLoadOptions.EntryListed
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveLoadOptions proprietà. Ottiene o imposta il delegato richiamato quando una voce è elencata nel sommario.
type: docs
weight: 50
url: /it/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Ottiene o imposta il delegato richiamato quando una voce è elencata nel sommario.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Esempi

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Guarda anche

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* spazio dei nomi [Aspose.Zip](../../archiveloadoptions/)
* assemblea [Aspose.Zip](../../../)


