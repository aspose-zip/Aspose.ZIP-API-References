---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento ZArchiveSaveOptions. Se dispara cuando se comprime una porción del flujo sin procesar"
type: docs
weight: 20
url: /es/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


