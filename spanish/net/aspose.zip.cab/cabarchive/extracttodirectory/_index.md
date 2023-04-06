---
title: CabArchive.ExtractToDirectory
second_title: Referencia de la API de Aspose.ZIP para .NET
description: CabArchive método. Extrae todos los archivos del archivo en el directorio proporcionado.
type: docs
weight: 40
url: /es/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

Extrae todos los archivos del archivo en el directorio proporcionado.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationDirectory | String | La ruta al directorio para colocar los archivos extraídos. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | la ruta es nula |
| PathTooLongException | La ruta especificada, el nombre de archivo o ambos superan la longitud máxima definida por el sistema. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder al directorio existente. |
| NotSupportedException | Si el directorio no existe, la ruta contiene un carácter de dos puntos (:) que no forma parte de la etiqueta de la unidad ("C:\"). |
| ArgumentException | ruta es una cadena de longitud cero, contiene solo espacios en blanco o contiene uno o más caracteres no válidos. Puede consultar caracteres no válidos mediante el método System.IO.Path.GetInvalidPathChars. -o- ruta tiene como prefijo, o contiene, solo un carácter de dos puntos (:). |
| IOException | El directorio especificado por ruta es un archivo. -o-- No se conoce el nombre de la red. |

### Observaciones

Si el directorio no existe, se creará.

### Ejemplos

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ver también

* class [CabArchive](../)
* espacio de nombres [Aspose.Zip.Cab](../../cabarchive/)
* asamblea [Aspose.Zip](../../../)


