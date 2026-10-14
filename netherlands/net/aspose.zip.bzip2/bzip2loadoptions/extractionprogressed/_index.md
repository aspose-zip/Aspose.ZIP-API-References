---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Bzip2LoadOptions event. Gebeurtenis die wordt opgewekt wanneer enkele bytes zijn geëxtraheerd."
type: docs
weight: 30
url: /nl/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Gebeurtenis die wordt opgewekt wanneer enkele bytes zijn geëxtraheerd.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Opmerkingen

Eventzender is de [`Bzip2Archive`](../../bzip2archive/) instantie waarvan de extractie is voortgeschreden. De [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) is het aantal bytes na extractie.

## Voorbeelden

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


