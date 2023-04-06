---
title: Class SevenZipArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.SevenZip.SevenZipArchive clase. Esta clase representa el archivo de almacenamiento 7z. Úselo para componer y extraer archivos 7z.
type: docs
weight: 660
url: /es/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Esta clase representa el archivo de almacenamiento 7z. Úselo para componer y extraer archivos 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Inicializa una nueva instancia del`SevenZipArchive` clase con configuraciones opcionales para sus entradas. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Inicializa una nueva instancia del`SevenZipArchive` La lista de entradas de clases y composiciones se puede extraer del archivo. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Inicializa una nueva instancia del`SevenZipArchive` La lista de entradas de clases y composiciones se puede extraer del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Obtiene entradas de[`SevenZipArchiveEntry`](../sevenziparchiveentry/) tipo que constituye el archivo. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Configuraciones de compresión y cifrado usadas para recién agregados[`SevenZipArchiveEntry`](../sevenziparchiveentry/) artículos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Crear entrada única dentro del archivo. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Extrae todos los archivos del archivo en el directorio proporcionado. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Guarda el archivo 7z en la secuencia proporcionada. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Guarda el archivo en el archivo de destino proporcionado. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Guarda el archivo de varios volúmenes en el directorio de destino proporcionado. |

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* espacio de nombres [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* asamblea [Aspose.Zip](../../)


