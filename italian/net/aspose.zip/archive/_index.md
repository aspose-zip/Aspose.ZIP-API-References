---
title: Class Archive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Archive classe. Questa classe rappresenta il file di archivio zip. Usalo per comporre estrarre o aggiornare archivi zip.
type: docs
weight: 10
url: /it/net/aspose.zip/archive/
---
## Archive class

Questa classe rappresenta il file di archivio zip. Usalo per comporre, estrarre o aggiornare archivi zip.

```csharp
public class Archive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Inizializza una nuova istanza di`Archive` classe con impostazioni facoltative per le sue voci. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Inizializza una nuova istanza di`Archive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Inizializza una nuova istanza di`Archive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Ottiene le voci di[`ArchiveEntry`](../archiveentry/) tipo che costituisce l'archivio. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Impostazioni di compressione e crittografia utilizzate per le nuove aggiunte[`ArchiveEntry`](../archiveentry/) articoli. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Rimuove la voce dall'elenco delle voci per indice. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Estrae tutti i file nell'archivio nella directory fornita. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Salva l'archivio nel file di destinazione fornito. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Salva l'archivio multivolume nella directory di destinazione fornita. |

### Guarda anche

* interface [IArchive](../iarchive/)
* spazio dei nomi [Aspose.Zip](../../aspose.zip/)
* assemblea [Aspose.Zip](../../)


