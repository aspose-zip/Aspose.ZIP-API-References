---
title: Class ArchiveEntryEncrypted
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.ArchiveEntryEncrypted clase. Entrada zip que debe comprimirse con cifrado o descomprimirse con descifrado.
type: docs
weight: 30
url: /es/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Entrada zip que debe comprimirse con cifrado o descomprimirse con descifrado.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Obtiene el comentario de la entrada dentro del archivo. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Obtiene el tamaño del archivo comprimido. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Obtiene la configuración de compresión o descompresión. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Obtiene la configuración de cifrado o descifrado. |
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


