---
title: "XarFileEntry.CompressionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento de XarFileEntry. Se genera cuando una porción del flujo sin procesar se comprime."
type: docs
weight: 20
url: /es/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Se lanza cuando una parte del flujo sin procesar se comprime.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Observaciones

El remitente del evento es una instancia [`XarFileEntry`](../).

## Ejemplos

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


