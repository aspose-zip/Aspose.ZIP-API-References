---
title: Archive.SaveSplit
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Archive método. Guarda el archivo de varios volúmenes en el directorio de destino proporcionado.
type: docs
weight: 100
url: /es/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Guarda el archivo de varios volúmenes en el directorio de destino proporcionado.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationDirectory | String | La ruta al directorio donde se crearán los segmentos de archivo. |
| options | SplitArchiveSaveOptions | Opciones para guardar archivos, incluido el nombre del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Este archivo fue abierto desde una fuente existente. |
| NotSupportedException | Este archivo está comprimido con el método XZ y encriptado. |
| ArgumentNullException | *destinationDirectory* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder al directorio. |
| ArgumentException | *destinationDirectory* contiene caracteres no válidos como ", &gt;, &lt; o &#x7C;. |
| PathTooLongException | La ruta especificada supera la longitud máxima definida por el sistema. |

### Observaciones

Este método compone varios (`norte`) archivos nombrearchivo.z01, nombrearchivo.z02, ..., nombrearchivo.z(n-1), nombrearchivo.zip.

No se puede hacer que el archivo existente sea de varios volúmenes.

### Ejemplos

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Ver también

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* espacio de nombres [Aspose.Zip](../../archive/)
* asamblea [Aspose.Zip](../../../)


