---
title: "GzipArchive.UncompressedSize"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad GzipArchive. Obtiene el tamaño de un archivo original."
type: docs
weight: 30
url: /es/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Obtiene el tamaño de un archivo original.

```csharp
public ulong UncompressedSize { get; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

Durante la descompresión, esta propiedad puede contener un tamaño incorrecto. Si el tamaño del archivo descomprimido supera los 4 GB, esta propiedad proporcionará un valor erróneo debido al límite de 32 bits en el encabezado.

### Ver también

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


