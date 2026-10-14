---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement LzmaArchiveSettings. Se déclenche lorsqu'une partie du flux brut est compressée"
type: docs
weight: 50
url: /fr/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Exemples

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


