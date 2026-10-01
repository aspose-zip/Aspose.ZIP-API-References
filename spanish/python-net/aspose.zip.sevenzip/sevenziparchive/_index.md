---
title: "SevenZipArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

Esta clase representa un archivo 7z. Úsela para crear y extraer archivos 7z.

El tipo SevenZipArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| SevenZipArchive(new_entry_settings) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) con configuraciones opcionales para sus entradas. |
| SevenZipArchive(source_stream, password) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) y compone una lista de entradas que puede extraerse del archivo. |
| SevenZipArchive(path, password) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) y compone una lista de entradas que puede extraerse del archivo. |
| SevenZipArchive(source_stream, options) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) y compone una lista de entradas que puede extraerse del archivo. |
| SevenZipArchive(path, options) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) y compone una lista de entradas que puede extraerse del archivo. |
| SevenZipArchive(parts, password) | Inicializa una nueva instancia de la clase [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) a partir de un archivo 7z de varios volúmenes y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| new_entry_settings | Configuraciones de compresión y cifrado utilizadas para los elementos [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) recién añadidos. |
| entries | Obtiene las entradas del tipo [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, new_entry_settings, file_info) | Crea una única entrada dentro del archivo. |
| create_entry(name, source, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entry(name, path, open_immediately, new_entry_settings) | Crea una única entrada dentro del archivo. |
| create_entries(directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio proporcionado. |
| create_entries(source_directory, include_root_directory) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio proporcionado. |
| save(output, save_options) | Guarda el archivo 7z en el flujo proporcionado. |
| save(destination_file_name, save_options) | Guarda el archivo en un archivo de destino proporcionado. |
| extract_to_directory(destination_directory, password) | Extrae todos los archivos del archivo al directorio proporcionado. |
| extract_to_directory(destination_directory) | Extrae todos los archivos del archivo al directorio proporcionado. |
| save_split(destination_directory, options) | Guarda el archivo multivolumen en el directorio de destino proporcionado. |

### Ver también

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

