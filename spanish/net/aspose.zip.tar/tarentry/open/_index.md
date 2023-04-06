---
title: TarEntry.Open
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarEntry método. Abre la entrada para la extracción y proporciona una secuencia con el contenido de la entrada.
type: docs
weight: 50
url: /es/net/aspose.zip.tar/tarentry/open/
---
## TarEntry.Open method

Abre la entrada para la extracción y proporciona una secuencia con el contenido de la entrada.

```csharp
public Stream Open()
```

### Valor_devuelto

La secuencia que representa el contenido de la entrada.

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
Stream decompressed = entry.Open();
```

### Ver también

* class [TarEntry](../)
* espacio de nombres [Aspose.Zip.Tar](../../tarentry/)
* asamblea [Aspose.Zip](../../../)


