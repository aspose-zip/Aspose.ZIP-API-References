---
title: Class GzipArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Gzip.GzipArchive clase. Esta clase representa el archivo de almacenamiento gzip. Úselo para componer o extraer archivos gzip.
type: docs
weight: 210
url: /es/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Esta clase representa el archivo de almacenamiento gzip. Úselo para componer o extraer archivos gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Inicializa una nueva instancia del`GzipArchive` clase preparada para comprimir. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Inicializa una nueva instancia del`GzipArchive` clase preparada para descomprimir. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Inicializa una nueva instancia del`GzipArchive` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Nombre del archivo original. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Extrae el archivo a la secuencia proporcionada. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Abre el archivo para su extracción y proporciona una secuencia con el contenido del archivo. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Guarda el archivo en la secuencia proporcionada. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Guarda el archivo en el archivo de destino proporcionado. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Establece el contenido que se comprimirá dentro del archivo. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Establece el contenido que se comprimirá dentro del archivo. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Establece el contenido que se comprimirá dentro del archivo. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Establece el contenido que se comprimirá dentro del archivo. |

### Observaciones

El algoritmo de compresión Gzip se basa en el algoritmo DEFLATE, que es una combinación de codificación LZ77 y Huffman.

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* espacio de nombres [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* asamblea [Aspose.Zip](../../)


