---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement ZArchiveLoadOptions. Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits"
type: docs
weight: 30
url: /fr/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarques

L'expéditeur de l'événement est l'instance [`ZArchive`](../../zarchive/) dont l'extraction progresse.

## Exemples

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


