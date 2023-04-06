---
title: GzipArchive.Extract
second_title: Referencia de la API de Aspose.ZIP para .NET
description: GzipArchive método. Extrae el archivo a la secuencia proporcionada.
type: docs
weight: 40
url: /es/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Extrae el archivo a la secuencia proporcionada.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destination | Stream | Flujo de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite la escritura. |

### Ejemplos

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Ver también

* class [GzipArchive](../)
* espacio de nombres [Aspose.Zip.Gzip](../../gziparchive/)
* asamblea [Aspose.Zip](../../../)


