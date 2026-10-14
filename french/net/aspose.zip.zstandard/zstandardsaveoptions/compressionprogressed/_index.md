---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Événement ZstandardSaveOptions. Se déclenche lorsqu'une partie du flux brut est compressée."
type: docs
weight: 20
url: /fr/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Exemples

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir aussi

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


