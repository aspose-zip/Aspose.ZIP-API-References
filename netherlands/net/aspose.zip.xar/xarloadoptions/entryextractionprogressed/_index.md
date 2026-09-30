---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarLoadOptions-eigenschap. Haalt op of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd."
type: docs
weight: 30
url: /nl/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Haalt op of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Opmerkingen

Afzender van het evenement is de [`XarFileEntry`](../../xarfileentry/) instantie waarvan de extractie vordert.

## Voorbeelden

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


