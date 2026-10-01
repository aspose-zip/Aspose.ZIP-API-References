---
title: "ZArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.z/zarchive/
---

## ZArchive class

Esta clase representa un archivo Z (compress). Úsela para crear o extraer archivos Z.

El tipo ZArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| ZArchive() | Inicializa una nueva instancia de la clase [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) preparada para comprimir. |
| ZArchive(source, load_options) | Inicializa una nueva instancia de la clase [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) preparada para descomprimir. |
| ZArchive(path, load_options) | Inicializa una nueva instancia de la clase [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) preparada para descomprimir. |
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
| extract(destination) | Extrae el archivo Z a un flujo. |
| extract(file_info) | Extrae el archivo Z a un archivo. |
| extract(path) | Extrae el archivo Z a un archivo por ruta. |
| save(output, settings) | Guarda el archivo xz en el flujo proporcionado. |
| save(destination_file_name, settings) | Guarda el archivo Z en el archivo de destino proporcionado. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(source_path) | Establece el contenido que se comprimirá dentro del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.z](/zip/python-net/aspose.zip.z/)
* assembly [Aspose.Zip](/zip/python-net/)

