---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement ZstandardLoadOptions. Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits."
type: docs
weight: 30
url: /fr/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Obtient ou définit le délégué invoqué lorsque certains octets ont été extraits.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarques

L'expéditeur de l'événement est l'instance [`ZstandardArchive`](../../zstandardarchive/) dont l'extraction progresse.

## Exemples

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


