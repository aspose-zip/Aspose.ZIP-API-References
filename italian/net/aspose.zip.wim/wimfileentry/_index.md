---
title: WimFileEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Rappresenta un singolo file allinterno dellarchivio wim.
type: docs
weight: 660
url: /it/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Rappresenta un singolo file all'interno dell'archivio wim.

```csharp
public sealed class WimFileEntry : WimEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams) { get; } | Ottiene i nomi dei flussi di dati alternativi per un file o una directory. |
| [Archive](../../aspose.zip.wim/wimentry/archive) { get; } | Ottiene l'archivio a cui appartiene la voce. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime) { get; } | Ottiene l'ultima volta che il file o la directory è stata modificata. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime) { get; } | Ottiene l'ora di creazione del file o della directory. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes) { get; } | Ottiene gli attributi del file o della directory. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath) { get; } | Ottiene il percorso completo della voce all'interno dell'immagine. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink) { get; } | Ottiene l'ID del collegamento fisico del file o della directory. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks) { get; } | Ottiene se il file o la directory è conosciuta con altri nomi. |
| [Image](../../aspose.zip.wim/wimentry/image) { get; } | Ottiene l'immagine a cui appartiene la voce. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory) { get; } | Ottiene un valore che indica se la voce rappresenta una directory. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime) { get; } | Ottiene l'ora dell'ultimo accesso al file o alla directory. |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime) { get; } | Ottiene l'ora di modifica del file o della directory. |
| [Length](../../aspose.zip.wim/wimfileentry/length) { get; } | Ottiene la lunghezza della voce in byte. |
| [Name](../../aspose.zip.wim/wimentry/name) { get; } | Ottiene il nome della voce all'interno dell'immagine. |
| [Parent](../../aspose.zip.wim/wimentry/parent) { get; } | Ottiene la directory padre a cui appartiene la voce. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname) { get; } | Ottiene il nome breve della voce all'interno dell'immagine. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract#extract_1)(Stream) | Estrae la voce nel flusso fornito. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract#extract)(string) | Estrae la voce nel filesystem dal percorso fornito. |
| [Open](../../aspose.zip.wim/wimfileentry/open)() | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring)() |  |

### Guarda anche

* class [WimEntry](../wimentry)
* spazio dei nomi [Aspose.Zip.Wim](../../aspose.zip.wim)
* assemblea [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->