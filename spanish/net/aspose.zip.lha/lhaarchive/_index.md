---
title: "Clase LhaArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Lha.LhaArchive. Esta clase representa un archivo LHA .lzh."
type: docs
weight: 630
url: /es/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Esta clase representa un archivo LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Inicializa una nueva instancia de la clase `LhaArchive` y compone una lista de entradas que pueden extraerse del archivo. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Inicializa una nueva instancia de la clase `LhaArchive` y compone una lista de entradas que pueden extraerse del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Obtiene las entradas de archivo del tipo [`LhaArchiveEntry`](../lhaarchiveentry/) que constituyen el archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extrae todos los archivos y directorios del archivo al directorio proporcionado. |

## Observaciones

Solo se admiten los siguientes métodos de compresión:

**Method**

**Explanation**

**lh0**

Sin comprimir

**lh4**

Diccionario deslizante de 8 KiB y Huffman estático

**lh5**

Diccionario deslizante de 16 KiB y Huffman estático

**lh6**

Diccionario deslizante de 64 KiB y Huffman estático

**lh7**

Diccionario deslizante de 128 KiB y Huffman estático

**lhx**

Diccionario deslizante de 1 Mib y Huffman estático

**lhd**

Directorio

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


