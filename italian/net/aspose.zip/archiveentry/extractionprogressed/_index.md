---
title: ArchiveEntry.ExtractionProgressed
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveEntry evento. Aumenta quando viene estratta una parte del flusso non elaborato.
type: docs
weight: 90
url: /it/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Aumenta quando viene estratta una parte del flusso non elaborato.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Osservazioni

Il mittente dell'evento è un[`ArchiveEntry`](../) esempio.

### Esempi

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Guarda anche

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* spazio dei nomi [Aspose.Zip](../../archiveentry/)
* assemblea [Aspose.Zip](../../../)


