---
title: "TarArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

Esta clase representa un archivo tar. Úsela para crear, extraer o actualizar archivos tar.

El tipo TarArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| TarArchive() | Inicializa una nueva instancia de la clase [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/). |
| TarArchive(source_stream) | Inicializa una nueva instancia de la clase [Archive](/zip/python-net/aspose.zip/archive/) y compone una lista de entradas que pueden extraerse del archivo. |
| TarArchive(path) | Inicializa una nueva instancia de la clase [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene las entradas del tipo [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, source, file_info) | Crea una única entrada dentro del archivo. |
| create_entry(name, file_info, open_immediately) | Crea una única entrada dentro del archivo. |
| create_entry(name, path, open_immediately) | Crea una única entrada dentro del archivo. |
| create_entries(directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| create_entries(source_directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| delete_entry(entry) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| delete_entry(entry_index) |  |
| save(output, format) |  |
| save(destination_file_name, format) |  |
| save_gzipped(output, format) |  |
| save_gzipped(path, format) |  |
| save_zstandard(output, format) |  |
| save_zstandard(path, format) |  |
| save_lzipped(output, format) |  |
| save_lzipped(path, format) |  |
| save_lzma_compressed(output, format) |  |
| save_lzma_compressed(path, format) |  |
| save_lz4_compressed(output, format) |  |
| save_lz4_compressed(path, format) |  |
| save_xz_compressed(output, format, settings) |  |
| save_xz_compressed(path, format, settings) |  |
| save_z_compressed(output, format) |  |
| save_z_compressed(path, format) |  |
| from_g_zip(source) | Extrae el archivo gzip suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_g_zip(path) | Extrae el archivo gzip suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_zstandard(source) | Extrae el archivo Zstandard suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_zstandard(path) | Extrae el archivo Zstandard suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_l_zip(source) | Extrae el archivo lzip suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_l_zip(path) | Extrae el archivo lzip suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_lzma(source) | Extrae el archivo LZMA suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_lzma(path) | Extrae el archivo LZMA suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_lz4(path) | Extrae el archivo LZ4 suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_lz4(source) | Extrae el archivo LZ4 suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_xz(source) | Extrae el archivo en formato xz suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_xz(path) | Extrae el archivo en formato xz suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_z(source) | Extrae el archivo Zstandard suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| from_z(path) | Extrae el archivo Zstandard suministrado y compone [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) a partir de los datos extraídos. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

