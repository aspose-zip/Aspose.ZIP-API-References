---
title: ArchiveEntry.CompressionProgressed
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveEntry evento. Aumenta quando viene compressa una parte del flusso non elaborato.
type: docs
weight: 80
url: /it/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Aumenta quando viene compressa una parte del flusso non elaborato.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Osservazioni

Il mittente dell'evento è un[`ArchiveEntry`](../) esempio.

### Esempi

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Guarda anche

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* spazio dei nomi [Aspose.Zip](../../archiveentry/)
* assemblea [Aspose.Zip](../../../)


