---
title: Class GzipArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Gzip.GzipArchive classe. Questa classe rappresenta il file di archivio gzip. Usalo per comporre o estrarre archivi gzip.
type: docs
weight: 210
url: /it/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Questa classe rappresenta il file di archivio gzip. Usalo per comporre o estrarre archivi gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Inizializza una nuova istanza di`GzipArchive` classe preparata per la compressione. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Inizializza una nuova istanza di`GzipArchive` classe preparata per la decompressione. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Inizializza una nuova istanza di`GzipArchive` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Nome del file originale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Estrae l'archivio nel flusso fornito. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Apre l'archivio per l'estrazione e fornisce un flusso con il contenuto dell'archivio. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Salva l'archivio nel file di destinazione fornito. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Imposta il contenuto da comprimere all'interno dell'archivio. |

### Osservazioni

L'algoritmo di compressione Gzip si basa sull'algoritmo DEFLATE, che è una combinazione della codifica LZ77 e Huffman.

### Guarda anche

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assemblea [Aspose.Zip](../../)


