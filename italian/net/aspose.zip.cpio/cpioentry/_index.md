---
title: Class CpioEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Cpio.CpioEntry classe. Rappresenta un singolo file allinterno dellarchivio cpio.
type: docs
weight: 170
url: /it/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

Rappresenta un singolo file all'interno dell'archivio cpio.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce rappresenta la directory. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | Ottiene l'ora dell'ultima scrittura. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | Ottiene la lunghezza della voce in byte. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | Ottiene il nome della voce all'interno dell'archivio. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | Ottiene l'archivio a cui appartiene la voce. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### Guarda anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assemblea [Aspose.Zip](../../)


