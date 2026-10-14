---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété XarLoadOptions. Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits"
type: docs
weight: 30
url: /fr/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Remarques

L'expéditeur de l'événement est l'instance [`XarFileEntry`](../../xarfileentry/) dont l'extraction progresse.

## Exemples

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


