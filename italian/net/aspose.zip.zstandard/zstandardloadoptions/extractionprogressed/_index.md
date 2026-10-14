---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento ZstandardLoadOptions. Ottiene o imposta il delegato invocato quando sono stati estratti alcuni byte"
type: docs
weight: 30
url: /it/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Osservazioni

Il mittente dell'evento è l'istanza [`ZstandardArchive`](../../zstandardarchive/) la cui estrazione è in corso.

## Esempi

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


