---
title: "Bzip2Archive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.bzip2/bzip2archive/
---

## Bzip2Archive class

Esta clase representa un archivo bzip2. Úsela para crear o extraer archivos bzip2.

El tipo Bzip2Archive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| Bzip2Archive() | Inicializa una nueva instancia de la clase [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) preparada para comprimir. |
| Bzip2Archive(source_stream, load_options) | Inicializa una nueva instancia de la clase [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) preparada para descomprimir. |
| Bzip2Archive(path, load_options) | Inicializa una nueva instancia de la clase [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) preparada para descomprimir. |
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
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(tar_archive, format) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(cpio_archive, format) | Establece el contenido que se comprimirá dentro del archivo. |
| extract(destination) | Extrae el archivo al flujo proporcionado. |
| extract(path) | Extrae el contenido del archivo al directorio proporcionado. |
| save(output_stream, save_options) | Guarda el archivo en el flujo proporcionado. |
| save(destination_file_name, save_options) | Guarda el archivo en un archivo de destino proporcionado. |
| open() | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |

### Ver también

* namespace [aspose.zip.bzip2](/zip/python-net/aspose.zip.bzip2/)
* assembly [Aspose.Zip](/zip/python-net/)

