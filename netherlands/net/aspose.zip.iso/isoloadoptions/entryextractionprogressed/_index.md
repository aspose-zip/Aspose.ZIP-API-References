---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoLoadOptions eigenschap. Haalt of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd"
type: docs
weight: 30
url: /nl/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Haalt op of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Opmerkingen

Afzender van het evenement is de [`IsoEntry`](../../isoentry/) instantie waarvan de extractie voortschrijdt.

## Voorbeelden

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


