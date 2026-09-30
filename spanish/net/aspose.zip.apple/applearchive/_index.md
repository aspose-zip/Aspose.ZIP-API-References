---
title: "Clase AppleArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.Apple.AppleArchive. Esta clase representa un archivo Apple Archive .aar. Úsela para crear archivos Apple Archive."
type: docs
weight: 60
url: /es/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Esta clase representa un archivo Apple Archive (.aar). Úsela para crear archivos Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Inicializa una nueva instancia de la clase `AppleArchive` con la configuración utilizada para las entradas compuestas. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Inicializa una nueva instancia de la clase `AppleArchive` y compone una lista de entradas que puede extraerse del archivo. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Inicializa una nueva instancia de la clase `AppleArchive` y compone una lista de entradas que puede extraerse del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Obtiene las entradas que constituyen el archivo. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Obtiene un valor que indica si el archivo utiliza compresión sólida. En modo sólido, todos los datos de las entradas se comprimen como una única secuencia y la extracción individual de entradas no está disponible. Use [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) en su lugar. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Obtiene la configuración utilizada para las nuevas entradas compuestas. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Crea una única entrada dentro del archivo. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Crea una única entrada dentro del archivo. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Crea una única entrada dentro del archivo. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Guarda el archivo en el flujo proporcionado. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Guarda el archivo en un archivo de destino proporcionado. |

## Observaciones

Apple y Apple Archive son marcas registradas de Apple Inc.

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


