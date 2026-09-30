---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà IsoLoadOptions. Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti."
type: docs
weight: 30
url: /it/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Osservazioni

Il mittente dell'evento è l'istanza [`IsoEntry`](../../isoentry/) la cui estrazione è in corso.

## Esempi

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


