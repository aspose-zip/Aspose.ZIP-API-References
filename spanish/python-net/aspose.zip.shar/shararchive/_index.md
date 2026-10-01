---
title: "SharArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.shar/shararchive/
---

## SharArchive class

Esta clase representa un archivo shar.

El tipo SharArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| SharArchive() | Inicializa una nueva instancia de la clase [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/). |
| SharArchive(path) | Inicializa una nueva instancia de la clase [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) preparada para descomprimir. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene entradas del tipo [SharEntry](/zip/python-net/aspose.zip.shar/sharentry/) que constituyen el archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entries(source_directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entries(directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entry(name, file_info, open_immediately) | Crea una única entrada dentro del archivo. |
| create_entry(name, source_path, open_immediately) | Crea una única entrada dentro del archivo. |
| create_entry(name, source) | Crea una única entrada dentro del archivo. |
| delete_entry(entry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| delete_entry(entry_index) |  |
| save(destination_file_name) | Guarda el archivo en un archivo de destino proporcionado. |
| save(output) | Guarda el archivo en el flujo proporcionado. |

### Ver también

* namespace [aspose.zip.shar](/zip/python-net/aspose.zip.shar/)
* assembly [Aspose.Zip](/zip/python-net/)

