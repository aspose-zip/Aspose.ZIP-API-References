---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZArchiveLoadOptions gebeurtenis. Haalt de delegate op of stelt deze in die wordt aangeroepen wanneer enkele bytes zijn uitgepakt"
type: docs
weight: 30
url: /nl/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Haalt op of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Opmerkingen

Afzender van de gebeurtenis is de [`ZArchive`](../../zarchive/) instantie waarvan de extractie vordert.

## Voorbeelden

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


