---
title: "Clase IsoArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Aspose.Zip.Iso.IsoArchive clase. Representa un archivo ISO ISO 9660"
type: docs
weight: 570
url: /es/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Representa un archivo ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Inicializa una nueva instancia de la clase `IsoArchive` y crea un archivo ISO vacío para agregar nuevos archivos y directorios. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Inicializa una nueva instancia de la clase `IsoArchive` y compone una lista de entradas que puede extraerse del archivo. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Inicializa una nueva instancia de la clase `IsoArchive` y compone una lista de entradas que puede extraerse del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Obtiene entradas del tipo [`IsoEntry`](../isoentry/) que constituyen el archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Agrega un directorio a la imagen ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Agrega un archivo a la imagen ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Agrega un archivo a la imagen ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Agrega un archivo a la imagen ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extrae todas las entradas al directorio especificado. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Guarda la imagen ISO en el flujo especificado. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Guarda la imagen ISO en la ruta especificada. |

### Ver también

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


