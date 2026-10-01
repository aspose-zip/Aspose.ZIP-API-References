---
title: "XarArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 40
url: /es/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

Esta clase representa un archivo xar.

El tipo XarArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| XarArchive(default_compression_settings) | Inicializa una nueva instancia de la clase [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/). |
| XarArchive(source_stream, load_options) | Inicializa una nueva instancia de la clase [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) y compone una lista de entradas que puede extraerse del archivo. |
| XarArchive(path, load_options) | Inicializa una nueva instancia de la clase [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene las entradas del tipo [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entries(directory, include_root_directory, compression_settings) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entry(name, file_info, open_immediately, compression_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source_path, open_immediately, compression_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, compression_settings) | Crea una única entrada dentro del archivo. |
| save(destination_file_name, save_options) | Guarda el archivo en el archivo de destino proporcionado. |
| save(output, save_options) | Guarda el archivo en el flujo proporcionado. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |
| delete_entry(entry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |

### Ver también

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

