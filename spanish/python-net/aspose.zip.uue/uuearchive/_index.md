---
title: "UueArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.uue/uuearchive/
---

## UueArchive class

Esta clase representa un archivo uuencoded.

El tipo UueArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| UueArchive() | Inicializa una nueva instancia de la clase [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) preparada para codificación. |
| UueArchive(source_stream) | Inicializa una nueva instancia de la clase [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) preparada para decodificar. |
| UueArchive(path) | Inicializa una nueva instancia de la clase [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/). |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| name | Nombre del archivo original. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| save(output_stream, save_options) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name, save_options) | Guarda el archivo en un archivo de destino proporcionado. |
| extract(destination) | Extrae el archivo al flujo proporcionado. |
| extract(path) | Extrae el archivo al archivo por ruta. |
| set_source(source) | Establece el contenido que se codificará dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se codificará dentro del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |
| open() | Abre el archivo para decodificar y proporciona un flujo con el contenido del archivo. |

### Ver también

* namespace [aspose.zip.uue](/zip/python-net/aspose.zip.uue/)
* assembly [Aspose.Zip](/zip/python-net/)

