---
title: Class SharArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Shar.SharArchive classe. Questa classe rappresenta il file di archivio shar.
type: docs
weight: 700
url: /it/net/aspose.zip.shar/shararchive/
---
## SharArchive class

Questa classe rappresenta il file di archivio shar.

```csharp
public class SharArchive : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | Inizializza una nuova istanza di`SharArchive` classe. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | Ottiene le voci di[`SharEntry`](../sharentry/) tipo che costituisce l'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | Crea una singola voce all'interno dell'archivio. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | Crea una singola voce all'interno dell'archivio. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | Rimuove la voce dall'elenco delle voci per indice. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | Salva l'archivio nello stream fornito. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | Salva l'archivio nel file di destinazione fornito. |

### Guarda anche

* spazio dei nomi [Aspose.Zip.Shar](../../aspose.zip.shar/)
* assemblea [Aspose.Zip](../../)


