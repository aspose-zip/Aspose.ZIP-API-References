---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveLoadOptions proprietà. Ottiene o imposta il delegato richiamato quando alcuni byte sono stati estratti.
type: docs
weight: 40
url: /it/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Ottiene o imposta il delegato richiamato quando alcuni byte sono stati estratti.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Osservazioni

Il mittente dell'evento è il[`ArchiveEntry`](../../archiveentry/) istanza in cui è in corso l'estrazione.

### Esempi

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Guarda anche

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* spazio dei nomi [Aspose.Zip](../../archiveloadoptions/)
* assemblea [Aspose.Zip](../../../)


