---
title: "CpioArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

Esta clase representa un archivo cpio.

El tipo CpioArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| CpioArchive() | Inicializa una nueva instancia de la clase [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/). |
| CpioArchive(source_stream) | Inicializa una nueva instancia de la clase [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) y compone una lista de entradas que puede extraerse del archivo. |
| CpioArchive(path) | Inicializa una nueva instancia de la clase [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene entradas del tipo [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
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
| save(destination_file_name, cpio_format) | Guarda el archivo en un archivo de destino proporcionado. |
| save(output, cpio_format) | Guarda el archivo en el flujo proporcionado. |
| save_gzipped(output, cpio_format) | Guarda el archivo en el flujo con compresión gzip. |
| save_gzipped(path, cpio_format) | Guarda el archivo en el archivo indicado por la ruta con compresión gzip. |
| save_lzipped(output, cpio_format) | Guarda el archivo en el flujo con compresión lzip. |
| save_lzipped(path, cpio_format) | Guarda el archivo en el archivo indicado por la ruta con compresión lzip. |
| save_lzma_compressed(output, cpio_format) | Guarda el archivo en el flujo con compresión LZMA. |
| save_lzma_compressed(path, cpio_format) | Guarda el archivo en el archivo indicado por la ruta con compresión lzma. |
| save_xz_compressed(output, cpio_format, settings) | Guarda el archivo en el flujo con compresión xz. |
| save_xz_compressed(path, cpio_format, settings) | Guarda el archivo en la ruta especificada con compresión xz. |
| save_z_compressed(output, cpio_format) | Guarda el archivo en el flujo con compresión Z. |
| save_z_compressed(path, cpio_format) | Guarda el archivo en la ruta con compresión Z. |
| save_zstandard(output, cpio_format) | Guarda el archivo en el flujo con compresión Zstandard. |
| save_zstandard(path, cpio_format) | Guarda el archivo en el archivo por ruta con compresión Zstandard. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

