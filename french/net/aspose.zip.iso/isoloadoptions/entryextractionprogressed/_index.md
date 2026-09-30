---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété IsoLoadOptions. Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits"
type: docs
weight: 30
url: /fr/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarques

L'expéditeur de l'événement est l'instance [`IsoEntry`](../../isoentry/) dont l'extraction progresse.

## Exemples

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


