---
title: Class ArchiveEntry
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.ArchiveEntry clase. Representa un solo archivo dentro del archivo.
type: docs
weight: 20
url: /es/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Representa un solo archivo dentro del archivo.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Obtiene el comentario de la entrada dentro del archivo. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Obtiene el tamaño del archivo comprimido. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Obtiene la configuración de compresión o descompresión. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Obtiene un valor que indica si la entrada representa el directorio. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Obtiene o establece la última fecha y hora de modificación. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Obtiene el nombre de la entrada dentro del archivo. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Obtiene el tamaño del archivo original. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Extrae la entrada al sistema de archivos por la ruta proporcionada. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Abre la entrada para su extracción y proporciona un flujo con contenido de entrada descomprimido. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Se genera cuando se comprime una parte del flujo sin procesar. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Se genera cuando se extrae una parte del flujo sin procesar. |

### Observaciones

Lanzar un`ArchiveEntry` instancia a[`ArchiveEntryEncrypted`](../archiveentryencrypted/) para determinar si la entrada está encriptada o no.

### Ver también

* interface [IArchiveFileEntry](../iarchivefileentry/)
* espacio de nombres [Aspose.Zip](../../aspose.zip/)
* asamblea [Aspose.Zip](../../)


