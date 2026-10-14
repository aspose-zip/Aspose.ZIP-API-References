---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad IsoLoadOptions. Obtiene o establece el delegado invocado cuando se han extraído algunos bytes"
type: docs
weight: 30
url: /es/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Obtiene o establece el delegado invocado cuando se han extraído algunos bytes.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Observaciones

El remitente del evento es la instancia [`IsoEntry`](../../isoentry/) cuya extracción está en progreso.

## Ejemplos

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


