---
title: Class SevenZipArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.SevenZip.SevenZipArchive classe. Questa classe rappresenta il file di archivio 7z. Usalo per comporre ed estrarre archivi 7z.
type: docs
weight: 660
url: /it/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Questa classe rappresenta il file di archivio 7z. Usalo per comporre ed estrarre archivi 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Inizializza una nuova istanza di`SevenZipArchive` classe con impostazioni facoltative per le sue voci. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Inizializza una nuova istanza di`SevenZipArchive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Inizializza una nuova istanza di`SevenZipArchive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Ottiene le voci di[`SevenZipArchiveEntry`](../sevenziparchiveentry/) tipo che costituisce l'archivio. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Impostazioni di compressione e crittografia utilizzate per le nuove aggiunte[`SevenZipArchiveEntry`](../sevenziparchiveentry/) articoli. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Crea una singola voce all'interno dell'archivio. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Estrae tutti i file nell'archivio nella directory fornita. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Salva l'archivio 7z nello stream fornito. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Salva l'archivio nel file di destinazione fornito. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Salva l'archivio multivolume nella directory di destinazione fornita. |

### Guarda anche

* interface [IArchive](../../aspose.zip/iarchive/)
* spazio dei nomi [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assemblea [Aspose.Zip](../../)


