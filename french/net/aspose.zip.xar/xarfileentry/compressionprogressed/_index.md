---
title: "XarFileEntry.CompressionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement XarFileEntry. Se déclenche lorsqu'une partie du flux brut est compressée"
type: docs
weight: 20
url: /fr/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Remarques

L'expéditeur de l'événement est une instance [`XarFileEntry`](../).

## Exemples

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


