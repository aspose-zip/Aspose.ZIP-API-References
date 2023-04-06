---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipArchiveEntry evento. Aumenta quando viene compressa una parte del flusso non elaborato.
type: docs
weight: 70
url: /it/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Aumenta quando viene compressa una parte del flusso non elaborato.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Osservazioni

Il mittente dell'evento è un[`SevenZipArchiveEntry`](../) esempio.

### Esempi

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Guarda anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assemblea [Aspose.Zip](../../../)


