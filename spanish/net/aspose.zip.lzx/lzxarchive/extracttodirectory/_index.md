---
title: "LzxArchive.ExtractToDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método LzxArchive. Extrae todos los archivos y directorios del archivo al directorio proporcionado"
type: docs
weight: 40
url: /es/net/aspose.zip.lzx/lzxarchive/extracttodirectory/
---
## LzxArchive.ExtractToDirectory method

Extrae todos los archivos y directorios del archivo al directorio proporcionado.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | String | La ruta al directorio donde se colocarán los archivos extraídos. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationDirectory* es nulo. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| SecurityException | El llamador no tiene el permiso requerido para acceder al directorio existente. |
| NotSupportedException | Si el directorio no existe, la ruta contiene un carácter de dos puntos (:) que no forma parte de una etiqueta de unidad (\"C:\\"). |
| ArgumentException | *destinationDirectory* es una cadena de longitud cero, contiene solo espacios en blanco, o contiene uno o más caracteres no válidos. Puede consultar los caracteres no válidos usando el método System.IO.Path.GetInvalidPathChars. -or- la ruta está precedida por, o contiene, solo un carácter de dos puntos (:). |
| IOException | El directorio especificado por path es un archivo. -or- El nombre de red no se conoce. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidDataException | Se ha proporcionado una contraseña incorrecta. - o - El archivo está corrupto. |
| NotSupportedException | Método de compresión no válido. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |

## Observaciones

Si el directorio no existe, se creará.

## Ejemplos

```csharp
using (var archive = new LzxArchive("archive.lzx")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ver también

* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


