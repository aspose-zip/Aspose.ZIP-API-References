---
title: "Clase ArjArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Arj.ArjArchive. Esta clase representa un archivo de archivo ARJ"
type: docs
weight: 250
url: /es/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Esta clase representa un archivo ARJ.

```csharp
public class ArjArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Inicializa una nueva instancia de la clase `ArjArchive` y compone una lista de entradas que pueden extraerse del archivo. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Inicializa una nueva instancia de la clase `ArjArchive` y compone una lista de entradas que pueden extraerse del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Obtiene el comentario. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Obtiene entradas del tipo [`ArjEntryPlain`](../arjentryplain/) que constituyen el archivo ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Obtiene el nombre original. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extrae todas las entradas al directorio especificado. |

## Observaciones

Solo se admiten los siguientes métodos de compresión:

**Method**

**Explanation**

**0**

Sin comprimir

**1**

Combinación de LZ77 y codificación Huffman adaptativa. Mejor relación.

**2**

Combinación de LZ77 y codificación Huffman adaptativa.

**3**

Combinación de LZ77 y codificación Huffman adaptativa. Mejor velocidad.

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


