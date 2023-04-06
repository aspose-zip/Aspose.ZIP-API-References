---
title: Class Bzip2Archive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Bzip2.Bzip2Archive classe. Questa classe rappresenta il file di archivio bzip2. Usalo per comporre o estrarre archivi bzip2.
type: docs
weight: 100
url: /it/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

Questa classe rappresenta il file di archivio bzip2. Usalo per comporre o estrarre archivi bzip2.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Inizializza una nuova istanza di`Bzip2Archive` classe preparata per la compressione. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream) | Inizializza una nuova istanza di`Bzip2Archive` classe preparata per la decompressione. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string) | Inizializza una nuova istanza di`Bzip2Archive` classe preparata per la decompressione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/)(Stream) | Estrae l'archivio nel flusso fornito. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Apre l'archivio per l'estrazione e fornisce un flusso con il contenuto dell'archivio. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Salva l'archivio nel file di destinazione fornito. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Imposta il contenuto da comprimere all'interno dell'archivio. |

### Osservazioni

bzip2 comprime i file utilizzando l'algoritmo di compressione del testo di ordinamento dei blocchi di Burrows-Wheeler e la codifica di Huffman. Per saperne di più: https://en.wikipedia.org/wiki/Bzip2

### Guarda anche

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assemblea [Aspose.Zip](../../)


