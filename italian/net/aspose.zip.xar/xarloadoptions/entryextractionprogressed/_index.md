---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà XarLoadOptions. Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti"
type: docs
weight: 30
url: /it/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Ottiene o imposta il delegato invocato quando alcuni byte sono stati estratti.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Osservazioni

Il mittente dell'evento è l'istanza [`XarFileEntry`](../../xarfileentry/) la cui estrazione è in corso.

## Esempi

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


