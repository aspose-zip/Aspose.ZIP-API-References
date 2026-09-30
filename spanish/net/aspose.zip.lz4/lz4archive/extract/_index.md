---
title: "Lz4Archive.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método Lz4Archive. Extrae el archivo al archivo mediante la ruta"
type: docs
weight: 30
url: /es/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extrae el archivo al archivo por ruta.

```csharp
public FileInfo Extract(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

### Valor devuelto

Información de un archivo extraído.

### Excepciones

| excepción | condición |
| --- | --- |
| EndOfStreamException | El flujo de origen es demasiado corto. |
| InvalidDataException | Se encontraron bytes incorrectos durante la decodificación. |
| NotSupportedException | Esta versión de LZ4 no es compatible. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | El archivo está preparado para la composición. |

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrae el archivo al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite escritura. |
| EndOfStreamException | El flujo de origen es demasiado corto. |
| InvalidDataException | Se encontraron bytes incorrectos durante la decodificación. |
| NotSupportedException | Esta versión de LZ4 no es compatible. |
| InvalidOperationException | El archivo está preparado para la composición. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


