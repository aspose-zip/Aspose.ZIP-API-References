---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento ZArchiveLoadOptions. Obtiene o establece el delegado invocado cuando se han extraído algunos bytes"
type: docs
weight: 30
url: /es/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Obtiene o establece el delegado invocado cuando se han extraído algunos bytes.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Observaciones

El remitente del evento es la instancia de [`ZArchive`](../../zarchive/) cuya extracción está en progreso.

## Ejemplos

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


