---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento ZArchiveLoadOptions. Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti"
type: docs
weight: 30
url: /it/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Osservazioni

Il mittente dell'evento è l'istanza [`ZArchive`](../../zarchive/) la cui estrazione è in corso.

## Esempi

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


