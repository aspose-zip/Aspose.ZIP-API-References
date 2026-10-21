---
title: "XzArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.xz/xzarchive/
---

## XzArchive class

Esta clase representa un archivo xz. Úsela para crear y extraer archivos xz.

El tipo XzArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| XzArchive(settings) | Inicializa una nueva instancia de la clase [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) y compone el archivo en formato xz. |
| XzArchive(source, options) | Inicializa una nueva instancia de la clase [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) preparada para descomprimir. |
| XzArchive(path, options) | Inicializa una nueva instancia de la clase [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) preparada para descomprimir. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| uncompressed_size | Tamaño sin comprimir de los datos del archivo en bytes. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
| name | Obtiene el nombre de la entrada. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| extract(destination) | Extrae el archivo xz a un flujo. |
| extract(file_info) | Extrae el archivo xz a un archivo. |
| extract(path) | Extrae el contenido del archivo al directorio proporcionado. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(source_path) | Establece el contenido que se comprimirá dentro del archivo. |
| save(output) | Guarda el archivo xz en el flujo proporcionado. |
| save(destination_file_name) | Guarda el archivo xz en el archivo de destino proporcionado. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.xz](/zip/python-net/aspose.zip.xz/)
* assembly [Aspose.Zip](/zip/python-net/)

