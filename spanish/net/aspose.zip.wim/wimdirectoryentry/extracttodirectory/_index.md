---
title: WimDirectoryEntry.ExtractToDirectory
second_title: Referencia de la API de Aspose.ZIP para .NET
description: WimDirectoryEntry método. Extrae todos los archivos del directorio actual al directorio proporcionado.
type: docs
weight: 50
url: /es/net/aspose.zip.wim/wimdirectoryentry/extracttodirectory/
---
## WimDirectoryEntry.ExtractToDirectory method

Extrae todos los archivos del directorio actual al directorio proporcionado.

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
| PathTooLongException | La ruta especificada, el nombre de archivo o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder al directorio existente. |
| NotSupportedException | Si el directorio no existe, la ruta contiene un carácter de dos puntos (:) que no forma parte de la etiqueta de la unidad ("C:\"). |
| ArgumentException | ruta es una cadena de longitud cero, contiene solo espacios en blanco o contiene uno o más caracteres no válidos. Puede consultar caracteres no válidos mediante el método System.IO.Path.GetInvalidPathChars. -o- ruta tiene como prefijo, o contiene, solo un carácter de dos puntos (:). |
| IOException | El directorio especificado por ruta es un archivo. -o-- No se conoce el nombre de la red. |

### Observaciones

Si el directorio no existe, se creará.

### Ejemplos

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].RootDirectory.ExtractToDirectory(@"C:\\extracted");
}
```

### Ver también

* class [WimDirectoryEntry](../)
* espacio de nombres [Aspose.Zip.Wim](../../wimdirectoryentry/)
* asamblea [Aspose.Zip](../../../)


