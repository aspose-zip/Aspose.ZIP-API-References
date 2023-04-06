---
title: Class TarArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Tar.TarArchive classe. Questa classe rappresenta il file di archivio tar. Usalo per comporre estrarre o aggiornare archivi tar.
type: docs
weight: 730
url: /it/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Questa classe rappresenta il file di archivio tar. Usalo per comporre, estrarre o aggiornare archivi tar.

```csharp
public class TarArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Inizializza una nuova istanza di`TarArchive` classe. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Inizializza una nuova istanza di[`Archive`](../../aspose.zip/archive/) classe e compone l'elenco delle voci può essere estratto dall'archivio. |
| [TarArchive](tararchive/#constructor_2)(string) | Inizializza una nuova istanza di`TarArchive` classe e compone l'elenco delle voci può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Ottiene le voci di[`TarEntry`](../tarentry/) tipo che costituisce l'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Estrae l'archivio gzip fornito e compone`TarArchive` dai dati estratti. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Estrae l'archivio gzip fornito e compone`TarArchive` dai dati estratti. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Estrae l'archivio lzip fornito e compone`TarArchive` dai dati estratti. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Estrae l'archivio lzip fornito e compone`TarArchive` dai dati estratti. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Estrae l'archivio in formato xz fornito e compone`TarArchive` dai dati estratti. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Estrae l'archivio in formato xz fornito e compone`TarArchive` dai dati estratti. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Estrae l'archivio in formato Z fornito e compone`TarArchive` dai dati estratti. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Estrae l'archivio in formato Z fornito e compone`TarArchive` dai dati estratti. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Crea una singola voce all'interno dell'archivio. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Rimuove la voce dall'elenco delle voci per indice. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Estrae tutti i file nell'archivio nella directory fornita. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Salva l'archivio nel file di destinazione fornito. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Salva l'archivio nello stream con compressione gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Salva l'archivio nel file per percorso con compressione gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Salva l'archivio nello stream con compressione lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Salva l'archivio nel file per percorso con compressione lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Salva l'archivio nello stream con compressione xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Salva l'archivio percorso per percorso con compressione xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Salva l'archivio nello stream con compressione Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Salva l'archivio percorso per percorso con compressione Z. |

### Guarda anche

* interface [IArchive](../../aspose.zip/iarchive/)
* spazio dei nomi [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assemblea [Aspose.Zip](../../)


