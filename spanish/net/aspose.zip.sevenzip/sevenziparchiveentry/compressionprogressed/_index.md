---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchiveEntry evento. Se genera cuando se comprime una parte del flujo sin procesar.
type: docs
weight: 70
url: /es/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Se genera cuando se comprime una parte del flujo sin procesar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Observaciones

El remitente del evento es un[`SevenZipArchiveEntry`](../) instancia.

### Ejemplos

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ver también

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* asamblea [Aspose.Zip](../../../)


