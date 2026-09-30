---
title: "AppleArchiveEntry.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método AppleArchiveEntry. Extrae la entrada al sistema de archivos usando la ruta proporcionada"
type: docs
weight: 50
url: /es/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

```csharp
public FileInfo Extract(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidDataException | La suma de verificación o digest almacenado para la entrada no coincide con los datos extraídos. |
| InvalidOperationException | La entrada pertenece a un archivo preparado para composición, o los datos de la entrada no pueden abrirse desde un flujo de archivo no buscable. |
| NotSupportedException | La entrada pertenece a un Apple Archive sólido o utiliza un método de compresión no compatible. |
| ObjectDisposedException | El flujo de origen ha sido eliminado. |
| IOException | Se produce un error de E/S. |

### Ver también

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrae la entrada al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destination* es `null`. |
| ArgumentException | *destination* no admite escritura. |
| InvalidDataException | La suma de verificación o digest almacenado para la entrada no coincide con los datos extraídos. |
| InvalidOperationException | La entrada pertenece a un archivo preparado para composición, o los datos de la entrada no pueden abrirse desde un flujo de archivo no buscable. |
| NotSupportedException | La entrada pertenece a un Apple Archive sólido o utiliza un método de compresión no compatible. |
| ObjectDisposedException | El flujo de origen ha sido eliminado. |
| IOException | Se produce un error de E/S. |

### Ver también

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


