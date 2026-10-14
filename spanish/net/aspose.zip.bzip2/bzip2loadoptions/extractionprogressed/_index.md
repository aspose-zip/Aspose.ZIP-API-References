---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento de Bzip2LoadOptions. Evento generado cuando se han extraído algunos bytes."
type: docs
weight: 30
url: /es/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Evento generado cuando se han extraído algunos bytes.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Observaciones

El remitente del evento es la instancia [`Bzip2Archive`](../../bzip2archive/) cuya extracción está en progreso. El [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) es el número de bytes después de la extracción.

## Ejemplos

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


