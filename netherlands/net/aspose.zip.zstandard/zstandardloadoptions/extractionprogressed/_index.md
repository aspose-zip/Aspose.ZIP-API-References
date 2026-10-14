---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZstandardLoadOptions gebeurtenis. Haalt op of stelt de delegate in die wordt aangeroepen wanneer er enkele bytes zijn geëxtraheerd."
type: docs
weight: 30
url: /nl/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Haalt op of stelt de delegate in die wordt aangeroepen wanneer enkele bytes zijn geëxtraheerd.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Opmerkingen

Afzender van het evenement is de [`ZstandardArchive`](../../zstandardarchive/) instantie waarvan de extractie is voortgeschreden.

## Voorbeelden

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


