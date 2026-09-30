---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento de LzmaArchiveSettings. Se genera cuando una porción del flujo sin procesar se comprime."
type: docs
weight: 50
url: /es/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Se lanza cuando una parte del flujo sin procesar se comprime.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Ejemplos

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


