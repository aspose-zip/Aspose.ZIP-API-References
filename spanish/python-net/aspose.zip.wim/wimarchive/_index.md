---
title: "WimArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.wim/wimarchive/
---

## WimArchive class

Esta clase representa un archivo wim.

El tipo WimArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| WimArchive(source_stream, load_options) | Inicializa una nueva instancia de la clase [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) y compone una lista de entradas que puede extraerse del archivo. |
| WimArchive(path, load_options) | Inicializa una nueva instancia de la clase [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| images | Obtiene las entradas del tipo [WimImage](/zip/python-net/aspose.zip.wim/wimimage/) que constituyen el archivo. |
| entries | Obtiene las entradas del tipo [WimEntry](/zip/python-net/aspose.zip.wim/wimentry/) que constituyen el archivo. |
| guid | Obtiene el GUID identificador del archivo. |
| boot_image_index | Obtiene el índice (basado en cero) de la imagen arrancable. |
| file_format_version | Obtiene la versión del formato de archivo. |
| manifest | Obtiene el manifiesto incrustado que describe el archivo y las imágenes contenidas. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| extract_to_directory(destination_directory) | Extrae el archivo al archivo por ruta. |

### Ver también

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

