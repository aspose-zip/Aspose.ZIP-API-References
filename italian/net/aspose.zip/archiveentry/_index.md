---
title: Class ArchiveEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.ArchiveEntry classe. Rappresenta un singolo file allinterno dellarchivio.
type: docs
weight: 20
url: /it/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Rappresenta un singolo file all'interno dell'archivio.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Ottiene il commento della voce all'interno dell'archivio. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Ottiene la dimensione del file compresso. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Ottiene le impostazioni per la compressione o la decompressione. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce rappresenta la directory. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Ottiene o imposta la data e l'ora dell'ultima modifica. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Ottiene il nome della voce all'interno dell'archivio. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Ottiene la dimensione del file originale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Aumenta quando viene compressa una parte del flusso non elaborato. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Aumenta quando viene estratta una parte del flusso non elaborato. |

### Osservazioni

Lancia un`ArchiveEntry` istanza a[`ArchiveEntryEncrypted`](../archiveentryencrypted/) per determinare se la voce è crittografata o meno.

### Guarda anche

* interface [IArchiveFileEntry](../iarchivefileentry/)
* spazio dei nomi [Aspose.Zip](../../aspose.zip/)
* assemblea [Aspose.Zip](../../)


