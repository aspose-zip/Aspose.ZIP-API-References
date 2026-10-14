---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento Bzip2SaveOptions. Se dispara cuando se comprime una porción del flujo sin procesar"
type: docs
weight: 40
url: /es/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Se lanza cuando una parte del flujo sin procesar se comprime.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Observaciones

Este evento no se disparará al comprimir en modo multihilo.

## Ejemplos

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


