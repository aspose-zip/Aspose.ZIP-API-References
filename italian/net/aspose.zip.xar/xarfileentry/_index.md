---
title: Class XarFileEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Xar.XarFileEntry classe. Rappresenta la voce del file allinterno dellarchivio xar.
type: docs
weight: 840
url: /it/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Rappresenta la voce del file all'interno dell'archivio xar.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Ottiene l'ora di creazione del file o della directory. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Ottiene il percorso completo della voce all'interno dell'archivio. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Ottiene un valore che indica se la voce rappresenta la directory. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Ottiene l'ora dell'ultimo accesso al file o alla directory. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Ottiene l'ora di modifica del file o della directory. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Ottiene la lunghezza della voce in byte. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Ottiene il nome della voce all'interno dell'archivio. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Ottiene la directory principale a cui appartiene la voce. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Estrae la voce nel flusso fornito. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Estrae la voce nel filesystem dal percorso fornito. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Guarda anche

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* spazio dei nomi [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assemblea [Aspose.Zip](../../)


