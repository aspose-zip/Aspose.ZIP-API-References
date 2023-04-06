---
title: Class SevenZipArchiveEntryPlain
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain clase. Entrada de SevenZip que debe comprimirse sin cifrar o descomprimirse sin descifrarse.
type: docs
weight: 690
url: /es/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

Entrada de SevenZip que debe comprimirse sin cifrar o descomprimirse sin descifrarse.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Obtiene el tamaño del archivo comprimido. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Obtiene la configuración de compresión o descompresión. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Obtiene un valor que indica si la entrada representa el directorio. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Obtiene la fecha y hora de última modificación. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Obtiene el nombre de la entrada dentro del archivo. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Obtiene el tamaño del archivo original. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Extrae la entrada al sistema de archivos por la ruta proporcionada. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Abre la entrada para la extracción y proporciona una secuencia con el contenido de la entrada. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Se genera cuando se comprime una parte del flujo sin procesar. |

### Ver también

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* espacio de nombres [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* asamblea [Aspose.Zip](../../)


