---
title: Bzip2Archive.Extract
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Bzip2Archive método. Extrae el archivo a la secuencia proporcionada.
type: docs
weight: 30
url: /es/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

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
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Ver también

* class [Bzip2Archive](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive/)
* asamblea [Aspose.Zip](../../../)


