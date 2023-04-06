---
title: Bzip2Archive.Open
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Bzip2Archive método. Abre el archivo para su extracción y proporciona una secuencia con el contenido del archivo.
type: docs
weight: 40
url: /es/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Abre el archivo para su extracción y proporciona una secuencia con el contenido del archivo.

```csharp
public Stream Open()
```

### Valor_devuelto

La secuencia que representa el contenido del archivo.

### Observaciones

Leer de la transmisión para obtener el contenido original del archivo. Ver sección de ejemplos.

### Ejemplos

Uso:

.NET 4.0 y superior: utilice el método Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 y anterior - copiar bytes manualmente:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = archive.Open();
```

### Ver también

* class [Bzip2Archive](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive/)
* asamblea [Aspose.Zip](../../../)


