---
title: "Classe AppleArchiveEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Apple.AppleArchiveEntry. Rappresenta una voce del filesystem all'interno di un AppleArchive"
type: docs
weight: 70
url: /it/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Rappresenta una voce del filesystem all'interno di un [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Restituisce un valore che indica se la voce rappresenta una directory. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Restituisce un valore che indica se la voce rappresenta un collegamento simbolico. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Restituisce la lunghezza non compressa della voce in byte. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Restituisce il percorso della voce all'interno dell'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Estrae la voce nello stream fornito. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Estrae la voce nel file system usando il percorso fornito. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |

## Osservazioni

Un'istanza di questa classe può rappresentare un file normale, una directory o un collegamento simbolico analizzato da un Apple Archive esistente, oppure un file o una directory aggiunti a un archivio in fase di composizione.

### Vedi anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


