---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento ZstandardSaveOptions. Se dispara cuando se comprime una porción del flujo sin procesar."
type: docs
weight: 20
url: /es/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Se lanza cuando una parte del flujo sin procesar se comprime.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Ejemplos

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


