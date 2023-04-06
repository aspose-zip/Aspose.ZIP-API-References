---
title: Class SevenZipArchiveEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry classe. Rappresenta un singolo file allinterno dellarchivio 7z.
type: docs
weight: 670
url: /it/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Rappresenta un singolo file all'interno dell'archivio 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Ottiene la dimensione del file compresso. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Ottiene le impostazioni per la compressione o la decompressione. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce rappresenta la directory. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Recupera la data e l'ora dell'ultima modifica. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Ottiene il nome della voce all'interno dell'archivio. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Ottiene la dimensione del file originale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Aumenta quando viene compressa una parte del flusso non elaborato. |

### Osservazioni

Lancia un`SevenZipArchiveEntry` istanza a[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) per determinare se la voce è crittografata o meno.

### Guarda anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assemblea [Aspose.Zip](../../)


