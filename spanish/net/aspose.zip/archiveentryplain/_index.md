---
title: Class ArchiveEntryPlain
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.ArchiveEntryPlain clase. Entrada zip que debe comprimirse sin cifrar o descomprimirse sin descifrar.
type: docs
weight: 40
url: /es/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

Entrada zip que debe comprimirse sin cifrar o descomprimirse sin descifrar.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
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
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extrae la entrada al sistema de archivos por la ruta proporcionada. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Abre la entrada para su extracción y proporciona un flujo con contenido de entrada descomprimido. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Se genera cuando se comprime una parte del flujo sin procesar. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Se genera cuando se extrae una parte del flujo sin procesar. |

### Ver también

* class [ArchiveEntry](../archiveentry/)
* espacio de nombres [Aspose.Zip](../../aspose.zip/)
* asamblea [Aspose.Zip](../../)


