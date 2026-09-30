---
title: "Clase EggEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Egg.EggEntry. Representa una entrada de archivo en un archivo EGG con todos sus metadatos"
type: docs
weight: 470
url: /es/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Representa una entrada de archivo en un archivo EGG con todos sus metadatos.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Obtiene el tamaño comprimido de la entrada. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Obtiene un valor que indica si esta entrada representa un directorio. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Obtiene o establece la fecha y hora de la última modificación. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Obtiene el nombre de la entrada dentro del archivo. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Obtiene el tamaño descomprimido de la entrada. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |

### Ver también

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


