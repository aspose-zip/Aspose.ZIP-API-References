---
title: RarArchiveEntry.ExtractionProgressed
second_title: Riferimento API Aspose.ZIP per .NET
description: RarArchiveEntry evento. Aumenta quando viene estratta una parte del flusso non elaborato.
type: docs
weight: 80
url: /it/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Aumenta quando viene estratta una parte del flusso non elaborato.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Osservazioni

Il mittente dell'evento è un[`RarArchiveEntry`](../) esempio.

### Esempi

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Guarda anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* spazio dei nomi [Aspose.Zip.Rar](../../rararchiveentry/)
* assemblea [Aspose.Zip](../../../)


