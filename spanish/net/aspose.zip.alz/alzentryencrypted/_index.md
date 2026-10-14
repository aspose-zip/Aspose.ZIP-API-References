---
title: "Clase AlzEntryEncrypted"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Alz.AlzEntryEncrypted. Entrada ALZ que necesita ser descifrada antes de la descompresión"
type: docs
weight: 40
url: /es/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

Entrada ALZ que necesita ser descifrada antes de la descompresión.

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Tamaño comprimido de los datos del archivo en bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Devuelve true si esta entrada representa un directorio. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Nombre de archivo (sin ruta). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Tamaño descomprimido de los datos del archivo en bytes. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Extrae la entrada al flujo proporcionado. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |

### Ver también

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


