---
title: "Classe EggEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Egg.EggEntry. Rappresenta una voce di file in un archivio EGG con tutti i suoi metadati"
type: docs
weight: 470
url: /it/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Rappresenta una voce di file in un archivio EGG con tutti i suoi metadati.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Restituisce la dimensione compressa della voce. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Restituisce un valore che indica se questa voce rappresenta una directory. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Ottiene o imposta la data e l'ora dell'ultima modifica. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Restituisce il nome della voce all'interno dell'archivio. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Restituisce la dimensione non compressa della voce. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Estrae la voce nello stream fornito. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Estrae la voce nel file system usando il percorso fornito. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Apre la voce per l'estrazione e fornisce uno stream con il contenuto decompresso della voce. |

### Vedi anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


