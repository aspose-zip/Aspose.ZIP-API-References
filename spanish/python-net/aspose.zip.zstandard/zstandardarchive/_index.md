---
title: "ZstandardArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.zstandard/zstandardarchive/
---

## ZstandardArchive class

Esta clase representa un archivo Zstandard. Úsela para crear archivos Zstandard.

El tipo ZstandardArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| ZstandardArchive() | Inicializa una nueva instancia de la clase [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) preparada para comprimir. |
| ZstandardArchive(source_stream, options) | Inicializa una nueva instancia de la clase [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) preparada para descomprimir. |
| ZstandardArchive(path, options) | Inicializa una nueva instancia de la clase [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/). |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
| name | Obtiene el nombre de la entrada. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| extract(destination) | Extrae el archivo al flujo proporcionado. |
| extract(path) | Extrae el archivo al archivo por ruta. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se comprimirá dentro del archivo. |
| save(output_stream, settings) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name, settings) | Guarda el archivo en el archivo de destino proporcionado. |
| save(destination, settings) | Guarda el archivo en el archivo de destino proporcionado. |
| open() | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.zstandard](/zip/python-net/aspose.zip.zstandard/)
* assembly [Aspose.Zip](/zip/python-net/)

