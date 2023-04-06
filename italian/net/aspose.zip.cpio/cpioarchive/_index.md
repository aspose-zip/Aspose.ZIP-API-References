---
title: Class CpioArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Cpio.CpioArchive classe. Questa classe rappresenta il file di archivio cpio.
type: docs
weight: 160
url: /it/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Questa classe rappresenta il file di archivio cpio.

```csharp
public class CpioArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Inizializza una nuova istanza di`CpioArchive` classe. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Inizializza una nuova istanza di`CpioArchive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Inizializza una nuova istanza di`CpioArchive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Ottiene le voci di[`CpioEntry`](../cpioentry/) tipo che costituisce l'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Crea una singola voce all'interno dell'archivio. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Rimuove la voce dall'elenco delle voci per indice. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Estrae tutti i file nell'archivio nella directory fornita. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Salva l'archivio nel file di destinazione fornito. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Salva l'archivio nello stream con compressione gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Salva l'archivio nel file per percorso con compressione gzip. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Salva l'archivio nello stream con compressione xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Salva l'archivio percorso per percorso con compressione xz. |

### Guarda anche

* interface [IArchive](../../aspose.zip/iarchive/)
* spazio dei nomi [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assemblea [Aspose.Zip](../../)


