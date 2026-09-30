---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement Bzip2LoadOptions. Événement déclenché lorsqu'un certain nombre d'octets ont été extraits"
type: docs
weight: 30
url: /fr/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Événement déclenché lorsqu'un certain nombre d'octets ont été extraits.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Remarques

L'expéditeur de l'événement est l'instance [`Bzip2Archive`](../../bzip2archive/) dont l'extraction progresse. Le [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) est le nombre d'octets après l'extraction.

## Exemples

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


