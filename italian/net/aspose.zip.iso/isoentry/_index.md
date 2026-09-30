---
title: "Classe IsoEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Iso.IsoEntry. Rappresenta un file o una directory di ingresso all'interno di un archivio ISO"
type: docs
weight: 580
url: /it/net/aspose.zip.iso/isoentry/
---
## IsoEntry class

Rappresenta una voce (file o directory) all'interno di un archivio ISO.

```csharp
public abstract class IsoEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsDirectory](../../aspose.zip.iso/isoentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce è una directory. |
| [Length](../../aspose.zip.iso/isoentry/length/) { get; } | Ottiene o imposta la data e l'ora di creazione. |
| [ModificationTime](../../aspose.zip.iso/isoentry/modificationtime/) { get; } | Ottiene o imposta la data e l'ora dell'ultima modifica. |
| [Name](../../aspose.zip.iso/isoentry/name/) { get; } | Ottiene il nome della voce. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract_1)(Stream) | Estrae la voce nello stream fornito. |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract)(string) | Estrae la voce nel file system usando il percorso fornito. |
| override [ToString](../../aspose.zip.iso/isoentry/tostring/)() | Restituisce una stringa che rappresenta la voce corrente. |

### Vedi anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


