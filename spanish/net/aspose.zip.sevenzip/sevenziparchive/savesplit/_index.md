---
title: SevenZipArchive.SaveSplit
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchive método. Guarda el archivo de varios volúmenes en el directorio de destino proporcionado.
type: docs
weight: 90
url: /es/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Guarda el archivo de varios volúmenes en el directorio de destino proporcionado.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationDirectory | String | La ruta al directorio donde se crearán los segmentos de archivo. |
| options | SplitSevenZipArchiveSaveOptions | Opciones para guardar archivos, incluido el nombre del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Este archivo fue abierto desde una fuente existente. |
| ArgumentNullException | *destinationDirectory* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder al directorio. |
| ArgumentException | *destinationDirectory* contiene caracteres no válidos como ", &gt;, &lt; o &#x7C;. |
| PathTooLongException | La ruta especificada supera la longitud máxima definida por el sistema. |

### Observaciones

Este método compone varios (`norte`) archivos filename.7z.001, filename.7z.002, ..., filename.7z.(n).

No se puede hacer que el archivo existente sea de varios volúmenes.

### Ejemplos

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Ver también

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)


