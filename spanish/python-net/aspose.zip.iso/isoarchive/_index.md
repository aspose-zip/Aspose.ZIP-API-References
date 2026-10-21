---
title: "IsoArchive"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 30
url: /es/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

Representa un archivo ISO (ISO 9660).

El tipo IsoArchive expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| IsoArchive() | Inicializa una nueva instancia de la clase [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) y crea un archivo ISO vacío<br/>             para agregar nuevos archivos y directorios. |
| IsoArchive(source_stream, load_options) | Inicializa una nueva instancia de la clase [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) y compone una lista de entradas que puede extraerse del archivo. |
| IsoArchive(path, load_options) | Inicializa una nueva instancia de la clase [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) y compone una lista de entradas que puede extraerse del archivo. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entries | Obtiene entradas del tipo [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) que constituyen el archivo. |
| file_entries | Obtiene entradas del tipo [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) que constituyen el archivo. |
| format | Obtiene el formato del archivo. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_entry(name, file_path) | Agrega un archivo a la imagen ISO. |
| create_entry(name, source) | Agrega un archivo a la imagen ISO. |
| create_entry(name) | Agrega un archivo a la imagen ISO. |
| save(path, save_options) | Guarda la imagen ISO en la ruta especificada. |
| save(stream, save_options) | Guarda la imagen ISO en el flujo especificado. |
| create_directory(name) | Agrega un directorio a la imagen ISO. |
| extract_to_directory(destination_directory) | Extrae todas las entradas al directorio especificado. |

### Ver también

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

