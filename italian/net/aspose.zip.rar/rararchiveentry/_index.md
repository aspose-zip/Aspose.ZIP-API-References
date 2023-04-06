---
title: Class RarArchiveEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Rar.RarArchiveEntry classe. Rappresenta un singolo file allinterno dellarchivio.
type: docs
weight: 320
url: /it/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Rappresenta un singolo file all'interno dell'archivio.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Ottiene la dimensione del file compresso. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Ottiene data e ora di creazione. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce rappresenta la directory. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Ottiene la data e l'ora dell'ultimo accesso. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Recupera la data e l'ora dell'ultima modifica. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Ottiene il nome della voce all'interno dell'archivio. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Ottiene la dimensione del file originale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Aumenta quando viene estratta una parte del flusso non elaborato. |

### Osservazioni

Lancia un`RarArchiveEntry` istanza a[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) per determinare se la voce è crittografata o meno.

### Guarda anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assemblea [Aspose.Zip](../../)


