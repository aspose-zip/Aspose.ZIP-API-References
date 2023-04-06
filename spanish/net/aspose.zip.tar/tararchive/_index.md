---
title: Class TarArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Tar.TarArchive clase. Esta clase representa el archivo tar. Úselo para componer extraer o actualizar archivos tar.
type: docs
weight: 730
url: /es/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Esta clase representa el archivo tar. Úselo para componer, extraer o actualizar archivos tar.

```csharp
public class TarArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Inicializa una nueva instancia del`TarArchive` clase. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Inicializa una nueva instancia del[`Archive`](../../aspose.zip/archive/) La lista de entradas de clases y composiciones se puede extraer del archivo. |
| [TarArchive](tararchive/#constructor_2)(string) | Inicializa una nueva instancia del`TarArchive` La lista de entradas de clases y composiciones se puede extraer del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Obtiene entradas de[`TarEntry`](../tarentry/) tipo que constituye el archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Extrae el archivo gzip suministrado y redacta`TarArchive` de datos extraídos. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Extrae el archivo gzip suministrado y redacta`TarArchive` de datos extraídos. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Extrae el archivo lzip proporcionado y redacta`TarArchive` de datos extraídos. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Extrae el archivo lzip proporcionado y redacta`TarArchive` de datos extraídos. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Extrae el archivo en formato xz suministrado y compone`TarArchive` de datos extraídos. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Extrae el archivo en formato xz suministrado y compone`TarArchive` de datos extraídos. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Extrae el archivo en formato Z proporcionado y compone`TarArchive` de datos extraídos. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Extrae el archivo en formato Z proporcionado y compone`TarArchive` de datos extraídos. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Crear entrada única dentro del archivo. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Elimina la entrada de la lista de entradas por index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Extrae todos los archivos del archivo en el directorio proporcionado. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Guarda el archivo en la secuencia proporcionada. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Guarda el archivo en el archivo de destino proporcionado. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Guarda el archivo en la transmisión con compresión gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Guarda el archivo en el archivo por ruta con compresión gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Guarda el archivo en la secuencia con compresión lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Guarda el archivo en el archivo por ruta con compresión lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Guarda el archivo en la secuencia con compresión xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Guarda el archivo en ruta por ruta con compresión xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Guarda el archivo en la secuencia con compresión Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Guarda el archivo en ruta por ruta con compresión Z. |

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* espacio de nombres [Aspose.Zip.Tar](../../aspose.zip.tar/)
* asamblea [Aspose.Zip](../../)


