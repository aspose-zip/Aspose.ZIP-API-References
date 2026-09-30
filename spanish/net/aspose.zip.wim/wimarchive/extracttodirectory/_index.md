---
title: "WimArchive.ExtractToDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método WimArchive. Extrae el archivo al archivo por ruta"
type: docs
weight: 90
url: /es/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Extrae el archivo al archivo por ruta.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | String | La ruta al directorio donde se colocarán los archivos extraídos. |

### Valor devuelto

Información del archivo extraído.

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *destinationDirectory* es nulo |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| SecurityException | El llamador no tiene el permiso requerido para acceder al directorio existente. |
| NotSupportedException | Si el directorio no existe, la ruta contiene un carácter de dos puntos (:) que no forma parte de una etiqueta de unidad (\"C:\\") - o - el archivo WIM es multiparte. |
| ArgumentException | path es una cadena de longitud cero, contiene solo espacios en blanco, o contiene uno o más caracteres no válidos. Puedes consultar los caracteres no válidos usando el método System.IO.Path.GetInvalidPathChars. -o- path tiene como prefijo, o contiene, solo un carácter de dos puntos (:). |
| IOException | El directorio especificado por path es un archivo. -or- El nombre de red no se conoce. |
| InvalidDataException | El archivo está corrupto. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |

### Ver también

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


