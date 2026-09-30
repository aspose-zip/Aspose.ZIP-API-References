---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad XarLoadOptions. Obtiene o establece el delegado invocado cuando se han extraído algunos bytes"
type: docs
weight: 30
url: /es/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Obtiene o establece el delegado invocado cuando se han extraído algunos bytes.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Observaciones

El remitente del evento es la instancia [`XarFileEntry`](../../xarfileentry/) cuya extracción está en progreso.

## Ejemplos

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


