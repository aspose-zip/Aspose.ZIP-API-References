---
title: Class RarArchiveEntryEncrypted
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Rar.RarArchiveEntryEncrypted clase. Entrada zip que debe descomprimirse con descifrado.
type: docs
weight: 330
url: /es/net/aspose.zip.rar/rararchiveentryencrypted/
---
## RarArchiveEntryEncrypted class

Entrada zip que debe descomprimirse con descifrado.

```csharp
public sealed class RarArchiveEntryEncrypted : RarArchiveEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Obtiene el tamaño del archivo comprimido. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Obtiene fecha y hora de creación. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Obtiene un valor que indica si la entrada representa el directorio. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Obtiene la fecha y hora del último acceso. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Obtiene la fecha y hora de última modificación. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Obtiene el nombre de la entrada dentro del archivo. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Obtiene el tamaño del archivo original. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | Extrae la entrada al sistema de archivos por la ruta proporcionada. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Abre la entrada para su extracción y proporciona un flujo con contenido de entrada descomprimido. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Se genera cuando se extrae una parte del flujo sin procesar. |

### Ver también

* class [RarArchiveEntry](../rararchiveentry/)
* espacio de nombres [Aspose.Zip.Rar](../../aspose.zip.rar/)
* asamblea [Aspose.Zip](../../)


