---
title: "Clase AppleArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Apple.AppleArchiveEntry. Representa una entrada del sistema de archivos dentro de un AppleArchive"
type: docs
weight: 70
url: /es/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Representa una entrada del sistema de archivos dentro de un [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Obtiene un valor que indica si la entrada representa un directorio. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Obtiene un valor que indica si la entrada representa un enlace simbólico. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Obtiene la longitud descomprimida de la entrada en bytes. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Obtiene la ruta de la entrada dentro del archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |

## Observaciones

Una instancia de esta clase puede representar un archivo regular, un directorio o un enlace simbólico analizado de un Apple Archive existente, o un archivo o directorio añadido a un archivo que se está creando.

### Ver también

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


