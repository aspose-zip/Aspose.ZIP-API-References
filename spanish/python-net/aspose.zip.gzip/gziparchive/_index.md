---
title: "GzipArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

Esta clase representa un archivo gzip. Úsela para crear o extraer archivos gzip.

El tipo GzipArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| GzipArchive() | Inicializa una nueva instancia de la clase [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) preparada para comprimir. |
| GzipArchive(source_stream, parse_header) | Inicializa una nueva instancia de la clase [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) preparada para descomprimir. |
| GzipArchive(source_stream, options) | Inicializa una nueva instancia de la clase [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) preparada para descomprimir. |
| GzipArchive(path, options) | Inicializa una nueva instancia de la clase [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) preparada para descomprimir. |
| GzipArchive(path, parse_header) | Inicializa una nueva instancia de la clase [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) preparada para descomprimir. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| uncompressed_size | Obtiene el tamaño de un archivo original. |
| name | Nombre del archivo original. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(tar_archive) | Establece el contenido que se comprimirá dentro del archivo. |
| extract(destination) | Extrae el archivo al flujo proporcionado. |
| extract(path) | Extrae el contenido del archivo al directorio proporcionado. |
| save(output_stream) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name) | Guarda el archivo en el archivo de destino proporcionado. |
| open() | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

