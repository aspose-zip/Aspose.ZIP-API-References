---
title: "Archive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip/archive/
---

## Archive class

Esta clase representa un archivo zip. Úsela para crear, extraer o actualizar archivos zip.

El tipo Archive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| Archive(new_entry_settings) | Inicializa una nueva instancia de la clase [Archive](/zip/python-net/aspose.zip/archive/) con configuraciones opcionales para sus entradas. |
| Archive(source_stream, load_options, new_entry_settings) | Inicializa una nueva instancia de la clase [Archive](/zip/python-net/aspose.zip/archive/) y compone una lista de entradas que pueden extraerse del archivo. |
| Archive(path, load_options, new_entry_settings) | Inicializa una nueva instancia de la clase [Archive](/zip/python-net/aspose.zip/archive/) y compone una lista de entradas que pueden extraerse del archivo. |
| Archive(main_segment, segments_in_order, load_options) | Inicializa una nueva instancia de la clase [Archive](/zip/python-net/aspose.zip/archive/) a partir de un archivo ZIP multivolumen y compone una lista de entradas que se puede extraer del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| new_entry_settings | Configuraciones de compresión y cifrado utilizadas para los elementos [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) recién añadidos. |
| comment | Obtiene el comentario del archivo completo. |
| entries | Obtiene las entradas de tipo [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, new_entry_settings, file_info) | Crea una única entrada dentro del archivo. |
| create_entries(directory, include_root_directory) | Añade al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entries(source_directory, include_root_directory) | Añade al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| delete_entry(entry) | Elimina la primera aparición de la entrada específica de la lista de entradas. |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name, save_options) | Guarda el archivo en el archivo de destino proporcionado. |
| save_split(destination_directory, options) | Guarda el archivo multivolumen en el directorio de destino proporcionado. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

