---
title: Class SharArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.Shar.SharArchive clase. Esta clase representa el archivo de almacenamiento compartido.
type: docs
weight: 700
url: /es/net/aspose.zip.shar/shararchive/
---
## SharArchive class

Esta clase representa el archivo de almacenamiento compartido.

```csharp
public class SharArchive : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | Inicializa una nueva instancia del`SharArchive` clase. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | Obtiene entradas de[`SharEntry`](../sharentry/) tipo que constituye el archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | Crear entrada única dentro del archivo. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | Crear entrada única dentro del archivo. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | Elimina la entrada de la lista de entradas por index. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | Guarda el archivo en la secuencia proporcionada. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | Guarda el archivo en el archivo de destino proporcionado. |

### Ver también

* espacio de nombres [Aspose.Zip.Shar](../../aspose.zip.shar/)
* asamblea [Aspose.Zip](../../)


