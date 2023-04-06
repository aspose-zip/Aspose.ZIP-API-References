---
title: RarArchiveEntry.ExtractionProgressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: RarArchiveEntry evento. Se genera cuando se extrae una parte del flujo sin procesar.
type: docs
weight: 80
url: /es/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Se genera cuando se extrae una parte del flujo sin procesar.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Observaciones

El remitente del evento es un[`RarArchiveEntry`](../) instancia.

### Ejemplos

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* espacio de nombres [Aspose.Zip.Rar](../../rararchiveentry/)
* asamblea [Aspose.Zip](../../../)


