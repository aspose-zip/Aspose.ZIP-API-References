---
title: "UueArchive.Open"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método UueArchive. Abre el archivo para decodificar y proporciona un flujo con el contenido del archivo."
type: docs
weight: 60
url: /es/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Abre el archivo para decodificar y proporciona un flujo con el contenido del archivo.

```csharp
public Stream Open()
```

### Valor devuelto

El flujo que representa el contenido del archivo.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

Lea del flujo para obtener el contenido original de un archivo. Consulte la sección de ejemplos.

## Ejemplos

Uso:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 y superiores - use el método Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 y anteriores - copie los bytes manualmente:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


