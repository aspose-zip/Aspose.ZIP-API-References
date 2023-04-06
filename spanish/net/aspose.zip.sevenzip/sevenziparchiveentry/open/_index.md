---
title: SevenZipArchiveEntry.Open
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchiveEntry método. Abre la entrada para la extracción y proporciona una secuencia con el contenido de la entrada.
type: docs
weight: 90
url: /es/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Abre la entrada para la extracción y proporciona una secuencia con el contenido de la entrada.

```csharp
public Stream Open(string password = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| password | String | Contraseña opcional para el descifrado. |

### Valor_devuelto

La secuencia que representa el contenido de la entrada.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | El archivo no está abierto para su extracción. - o - Esta entrada es un directorio. |
| InvalidDataException | Datos incorrectos dentro de la entrada. |

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

* class [SevenZipArchiveEntry](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* asamblea [Aspose.Zip](../../../)


