---
title: Class SevenZipArchiveEntryPlain
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain classe. Voce SevenZip che deve essere compressa senza crittografia o decompressa senza decrittografia.
type: docs
weight: 690
url: /it/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

Voce SevenZip che deve essere compressa senza crittografia o decompressa senza decrittografia.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Aumenta quando viene compressa una parte del flusso non elaborato. |

### Guarda anche

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* spazio dei nomi [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assemblea [Aspose.Zip](../../)


