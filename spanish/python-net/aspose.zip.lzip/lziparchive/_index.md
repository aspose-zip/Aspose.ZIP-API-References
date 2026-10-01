---
title: "LzipArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.lzip/lziparchive/
---

## LzipArchive class

Esta clase representa un archivo Lzip. Úsela para crear o extraer archivos Lzip.

El tipo LzipArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| LzipArchive(settings) | Inicializa una nueva instancia de [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/). |
| LzipArchive(source_stream, options) | Inicializa una nueva instancia de la clase [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) preparada para descomprimir. |
| LzipArchive(path, options) | Inicializa una nueva instancia de la clase [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) preparada para descomprimir. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| uncompressed_size | Tamaño sin comprimir de los datos del archivo en bytes. |
| settings | Obtiene la configuración de un archivo lzip particular. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
| name | Obtiene el nombre de la entrada. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| extract(destination) | Extrae el archivo lzip a un flujo. |
| extract(file_info) | Extrae el archivo lzip a un archivo. |
| extract(path) | Extrae el archivo lzip a un archivo mediante la ruta. |
| save(output_stream) | Guarda el archivo lzip en el flujo proporcionado. |
| save(destination_file_name) | Guarda el archivo lzip en el archivo de destino proporcionado. |
| save(destination) | Guarda el archivo lzip en el archivo de destino proporcionado. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se comprimirá dentro del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.lzip](/zip/python-net/aspose.zip.lzip/)
* assembly [Aspose.Zip](/zip/python-net/)

