---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement Bzip2SaveOptions. Se déclenche lorsqu'une partie du flux brut est compressée"
type: docs
weight: 40
url: /fr/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarques

Cet événement ne sera pas déclenché lors de la compression en mode multithread.

## Exemples

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


