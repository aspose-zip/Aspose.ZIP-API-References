---
title: "AlzEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa una entrada de archivo en un archivo ALZ junto con sus metadatos."
type: docs
weight: 13
url: /es/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Representa una entrada de archivo en un archivo ALZ junto con sus metadatos.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada a un flujo escribible. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrae la entrada a un flujo escribible usando una contraseña opcional. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al archivo especificado. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrae la entrada al archivo especificado usando una contraseña opcional. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño comprimido de los datos de la entrada en bytes. |
| [getLength()](#getLength--) | Obtiene la longitud descomprimida de esta entrada. |
| [getName()](#getName--) | Obtiene el nombre de la entrada almacenado en el archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño descomprimido de los datos de la entrada en bytes. |
| [isDirectory()](#isDirectory--) | Obtiene si esta entrada representa un directorio. |
| [open()](#open--) | Abre la entrada y proporciona un flujo que contiene datos descomprimidos. |
| [open(String password)](#open-java.lang.String-) | Abre la entrada y proporciona un flujo que contiene datos descomprimidos. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada a un flujo escribible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extrae la entrada a un flujo escribible usando una contraseña opcional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino |
| contraseña | java.lang.String | contraseña opcional para esta entrada |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae la entrada al archivo especificado. Un archivo existente se sobrescribe.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | ruta del archivo de destino |

**Returns:**
java.io.File - archivo extraído
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extrae la entrada al archivo especificado usando una contraseña opcional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | ruta del archivo de destino |
| contraseña | java.lang.String | contraseña opcional para esta entrada |

**Returns:**
java.io.File - archivo extraído
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtiene el tamaño comprimido de los datos de la entrada en bytes.

**Returns:**
long - tamaño comprimido en bytes
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtiene la longitud descomprimida de esta entrada.

**Returns:**
java.lang.Long - longitud descomprimida en bytes
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada almacenado en el archivo.

**Returns:**
java.lang.String - nombre de la entrada
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtiene el tamaño descomprimido de los datos de la entrada en bytes.

**Returns:**
long - tamaño descomprimido en bytes
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtiene si esta entrada representa un directorio.

**Returns:**
boolean - `true` para una entrada de directorio
### open() {#open--}
```
public final InputStream open()
```


Abre la entrada y proporciona un flujo que contiene datos descomprimidos.

**Returns:**
java.io.InputStream - flujo que contiene los datos descomprimidos de la entrada
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Abre la entrada y proporciona un flujo que contiene datos descomprimidos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | java.lang.String | contraseña opcional para esta entrada |

**Returns:**
java.io.InputStream - flujo que contiene los datos descomprimidos de la entrada
