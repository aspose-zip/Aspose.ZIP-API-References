---
title: "IsoEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo o directorio de entrada dentro de un archivo ISO."
type: docs
weight: 72
url: /es/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Representa una entrada (archivo o directorio) dentro de un archivo ISO.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada. |
| [getModificationTime()](#getModificationTime--) | Obtiene la fecha y hora de la última modificación. |
| [getName()](#getName--) | Obtiene el nombre de la entrada. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada es un directorio. |
| [toString()](#toString--) | Devuelve una cadena que representa la entrada actual. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito |

**Returns:**
java.io.File - instancia de java.io.File que contiene los datos extraídos
### getLength() {#getLength--}
```
public Long getLength()
```


Obtiene la longitud de la entrada.

**Returns:**
java.lang.Long - la longitud de la entrada
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtiene la fecha y hora de la última modificación.

**Returns:**
java.util.Date - fecha y hora de la última modificación
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada.

**Returns:**
java.lang.String - el nombre de la entrada
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtiene un valor que indica si la entrada es un directorio.

**Returns:**
boolean - un valor que indica si la entrada representa un directorio
### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa la entrada actual.

**Returns:**
java.lang.String - el nombre de la entrada
