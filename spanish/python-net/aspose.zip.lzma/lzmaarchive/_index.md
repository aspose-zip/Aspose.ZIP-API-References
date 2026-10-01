---
title: "LzmaArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.lzma/lzmaarchive/
---

## LzmaArchive class

Esta clase representa un archivo LZMA. Úsela para crear o extraer archivos LZMA.

El tipo LzmaArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| LzmaArchive(settings) | Inicializa una nueva instancia de la clase [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) y crea el archivo en formato lzma. |
| LzmaArchive(source) | Inicializa una nueva instancia de la clase [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) preparada para descomprimir. |
| LzmaArchive(path) | Inicializa una nueva instancia de la clase [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) preparada para descomprimir. |
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
| extract(destination) | Extrae el archivo lzma a un flujo. |
| extract(file_info) | Extrae el archivo lzma a un archivo. |
| extract(path) | Extrae el archivo lzma a un archivo por ruta. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(source_path) | Establece el contenido que se comprimirá dentro del archivo. |
| save(output) | Guarda el archivo lzma en el flujo proporcionado. |
| save(destination) | Guarda el archivo lzma en el archivo de destino proporcionado. |
| save(destination_file_name) | Guarda el archivo lzma en el archivo de destino proporcionado. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.lzma](/zip/python-net/aspose.zip.lzma/)
* assembly [Aspose.Zip](/zip/python-net/)

