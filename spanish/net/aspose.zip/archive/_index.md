---
title: Class Archive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Archive clase. Esta clase representa un archivo zip. Úselo para componer extraer o actualizar archivos zip.
type: docs
weight: 10
url: /es/net/aspose.zip/archive/
---
## Archive class

Esta clase representa un archivo zip. Úselo para componer, extraer o actualizar archivos zip.

```csharp
public class Archive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Inicializa una nueva instancia del`Archive` clase con configuraciones opcionales para sus entradas. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Inicializa una nueva instancia del`Archive` La lista de entradas de clases y composiciones se puede extraer del archivo. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Inicializa una nueva instancia del`Archive` La lista de entradas de clases y composiciones se puede extraer del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Obtiene entradas de[`ArchiveEntry`](../archiveentry/) tipo que constituye el archivo. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Configuraciones de compresión y cifrado usadas para recién agregados[`ArchiveEntry`](../archiveentry/) artículos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Crear entrada única dentro del archivo. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Elimina la entrada de la lista de entradas por index. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Extrae todos los archivos del archivo en el directorio proporcionado. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Guarda el archivo en la secuencia proporcionada. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Guarda el archivo en el archivo de destino proporcionado. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Guarda el archivo de varios volúmenes en el directorio de destino proporcionado. |

### Ver también

* interface [IArchive](../iarchive/)
* espacio de nombres [Aspose.Zip](../../aspose.zip/)
* asamblea [Aspose.Zip](../../)


