---
title: "ArchiveEntryEncrypted"
second_title: "Referencia de API de Aspose.Zip para Python a través de .NET"
description: 
type: docs
weight: 30
url: /es/python-net/aspose.zip/archiveentryencrypted/
---

## ArchiveEntryEncrypted class

Entrada zip que necesita ser comprimida con cifrado o descomprimida con descifrado.

El tipo ArchiveEntryEncrypted expone los siguientes miembros:
## Propiedades
| Nombre | Descripción |
| :- | :- |
| compressed_size | Obtiene el tamaño del archivo comprimido. |
| name | Obtiene el nombre de la entrada dentro del archivo. |
| comment | Obtiene el comentario de la entrada dentro del archivo. |
| uncompressed_size | Obtiene el tamaño del archivo original. |
| modification_time | Obtiene o establece la fecha y hora de la última modificación. |
| is_directory | Obtiene un valor que indica si la entrada representa un directorio. |
| data_source | Origen de la entrada si la entrada fue añadida al archivo, no extraída. |
| compression_settings | Obtiene la configuración para compresión o descompresión. |
| encryption_settings | Obtiene la configuración para cifrado o descifrado. |
| length | Obtiene la longitud de la entrada en bytes. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| extract(path, password) | Extrae la entrada al sistema de archivos usando la ruta proporcionada. |
| extract(destination, password) | Extrae la entrada al flujo proporcionado. |
| extract(path) | Extrae la entrada al sistema de archivos usando la ruta proporcionada. |
| extract(destination) | Extrae la entrada al flujo proporcionado. |
| open(password) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |

### Ver también

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

