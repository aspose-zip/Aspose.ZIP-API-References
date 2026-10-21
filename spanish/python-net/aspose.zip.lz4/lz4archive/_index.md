---
title: "Lz4Archive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 10
url: /es/python-net/aspose.zip.lz4/lz4archive/
---

## Lz4Archive class

Esta clase representa un archivo LZ4. Úsela para extraer o crear archivos LZ4.

El tipo Lz4Archive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| Lz4Archive(source_stream, load_options) | Inicializa una nueva instancia de la clase [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) preparada para descomprimir. |
| Lz4Archive(path, load_options) | Inicializa una nueva instancia de la clase [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/). |
| Lz4Archive(settings) | Inicializa una nueva instancia de la clase [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) preparada para comprimir. |
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
| extract(path) | Extrae el archivo al archivo por ruta. |
| extract(destination) | Extrae el archivo al flujo proporcionado. |
| save(output) | Guarda el archivo lz4 en el flujo proporcionado. |
| save(destination) | Guarda el archivo lz4 en el archivo de destino proporcionado. |
| save(destination_file_name) | Guarda el archivo en el archivo de destino proporcionado. |
| set_source(source) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(file_info) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(tar_archive, format) | Establece el contenido que se comprimirá dentro del archivo. |
| set_source(path) | Establece el contenido que se comprimirá dentro del archivo. |
| extract_to_directory(destination_directory) | Extrae el contenido del archivo al directorio proporcionado. |
| open() | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |

### Ver también

* namespace [aspose.zip.lz4](/zip/python-net/aspose.zip.lz4/)
* assembly [Aspose.Zip](/zip/python-net/)

