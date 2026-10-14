---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Evento ZstandardLoadOptions. Obtiene o establece el delegado invocado cuando se han extraído algunos bytes."
type: docs
weight: 30
url: /es/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Obtiene o establece el delegado invocado cuando se han extraído algunos bytes.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Observaciones

El remitente del evento es la instancia [`ZstandardArchive`](../../zstandardarchive/) cuya extracción está en progreso.

## Ejemplos

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


