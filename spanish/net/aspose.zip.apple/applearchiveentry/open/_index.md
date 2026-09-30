---
title: "AppleArchiveEntry.Open"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método AppleArchiveEntry. Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada"
type: docs
weight: 60
url: /es/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada.

```csharp
public Stream Open()
```

### Valor devuelto

Un flujo legible que contiene los datos extraídos de la entrada.

### Excepciones

| excepción | condición |
| --- | --- |
| NotSupportedException | La entrada pertenece a un Apple Archive sólido o utiliza un método de compresión no compatible. |
| InvalidDataException | La suma de verificación o digest almacenado para la entrada no coincide con los datos extraídos. |
| InvalidOperationException | La entrada pertenece a un archivo preparado para composición, o los datos de la entrada no pueden abrirse desde un flujo de archivo no buscable. |
| ObjectDisposedException | El flujo de origen ha sido eliminado. |
| IOException | Se produce un error de E/S. |

## Observaciones

Lea del flujo devuelto para obtener el contenido original de la entrada. Si el archivo contiene campos de suma de verificación, la suma se verifica mientras se lee el flujo devuelto.

### Ver también

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


