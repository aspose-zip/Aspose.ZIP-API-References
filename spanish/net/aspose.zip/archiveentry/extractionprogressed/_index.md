---
title: ArchiveEntry.ExtractionProgressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ArchiveEntry evento. Se genera cuando se extrae una parte del flujo sin procesar.
type: docs
weight: 90
url: /es/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Se genera cuando se extrae una parte del flujo sin procesar.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Observaciones

El remitente del evento es un[`ArchiveEntry`](../) instancia.

### Ejemplos

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Ver también

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* espacio de nombres [Aspose.Zip](../../archiveentry/)
* asamblea [Aspose.Zip](../../../)


