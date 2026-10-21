---
title: "CabArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

Esta clase representa un archivo CAB.

El tipo CabArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| CabArchive(settings) | Inicializa una nueva instancia de la clase [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) preparada para comprimir. |
| CabArchive(source_stream, load_options) | Inicializa una nueva instancia de la clase [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) y compone una lista de entradas que puede extraerse del archivo. |
| CabArchive(path, load_options) | Inicializa una nueva instancia de la clase [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene entradas del tipo [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, path, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, file_info, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entries(directory, include_root_directory) | Agrega al archivo todos los archivos, de forma recursiva, desde el directorio especificado. |
| create_entries(source_directory, include_root_directory) | Agrega al archivo todos los archivos de forma recursiva desde la ruta del directorio especificado. |
| save(output_stream, save_options) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name, save_options) | Guarda el archivo en el archivo de destino proporcionado. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

