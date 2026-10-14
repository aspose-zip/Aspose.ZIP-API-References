---
title: "ArchiveFactory.CompressDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método ArchiveFactory. Comprime el directorio especificado en un archivo de archivo utilizando el formato de archivo proporcionado."
type: docs
weight: 10
url: /es/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Comprime el directorio especificado en un archivo de archivo utilizando el formato de archivo proporcionado.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al directorio que será comprimido. |
| outputFileName | String | Nombre de archivo de destino. |
| archiveFormat | ArchiveFormat | El formato del archivo a crear (p. ej., zip, rar, tar, etc.). |

### Excepciones

| excepción | condición |
| --- | --- |
| DirectoryNotFoundException | Se lanza si el directorio especificado por *path* no existe. |
| ArgumentException | Se lanza si *path* es nulo o una cadena vacía. |
| NotSupportedException | Se lanza si el *archiveFormat* especificado no es compatible o no se reconoce. |
| ArgumentNullException | *path* es `null`. |

## Observaciones

Este método creará un archivo de archivo en la ubicación especificada por el parámetro *path*. El nombre del archivo de archivo será típicamente el nombre del directorio seguido de la extensión de archivo apropiada basada en *archiveFormat*. El propio directorio no se modifica ni se elimina.

## Ejemplos

Aquí hay un ejemplo de cómo usar el método CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Esto creará un archivo ZIP con el contenido del directorio en la ruta especificada.
```

### Ver también

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


