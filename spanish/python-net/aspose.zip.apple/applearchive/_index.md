---
title: "AppleArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

Esta clase representa un archivo Apple Archive (.aar). Úsela para crear archivos Apple Archive.

El tipo AppleArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| AppleArchive(new_entry_settings) | Inicializa una nueva instancia de la clase [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) con la configuración usada para entradas compuestas. |
| AppleArchive(source_stream, load_options) | Inicializa una nueva instancia de la clase [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) y compone una lista de entradas que puede extraerse del archivo. |
| AppleArchive(path, load_options) | Inicializa una nueva instancia de la clase [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entradas | Obtiene las entradas que constituyen el archivo. |
| is_solid | Obtiene un valor que indica si el archivo utiliza compresión sólida.<br/>            En modo sólido, todos los datos de la entrada se comprimen como una única secuencia y<br/>            la extracción individual de entradas no está disponible. Use |
| new_entry_settings | Obtiene la configuración utilizada para entradas recién compuestas. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, path, open_immediately) | Crea una única entrada dentro del archivo. |
| create_entry(name, source) | Crea una única entrada dentro del archivo. |
| create_entry(name, file_info, open_immediately) | Crea una única entrada dentro del archivo. |
| save(output) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name) | Guarda el archivo en un archivo de destino proporcionado. |
| create_entries(directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio proporcionado. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

