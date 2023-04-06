---
title: ArchiveEntry.CompressionProgressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ArchiveEntry evento. Se genera cuando se comprime una parte del flujo sin procesar.
type: docs
weight: 80
url: /es/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Se genera cuando se comprime una parte del flujo sin procesar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Observaciones

El remitente del evento es un[`ArchiveEntry`](../) instancia.

### Ejemplos

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* espacio de nombres [Aspose.Zip](../../archiveentry/)
* asamblea [Aspose.Zip](../../../)


