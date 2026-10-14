---
title: "IArchiveFileEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta interfaz representa una entrada de archivo."
type: docs
weight: 162
url: /es/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Esta interfaz representa una entrada de archivo.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getName()](#getName--) | Obtiene el nombre de la entrada. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino. Debe ser escribible |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

**Returns:**
java.io.File - instancia de java.io.File que contiene los datos extraídos
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Obtiene la longitud de la entrada en bytes.

**Returns:**
java.lang.Long - la longitud de la entrada en bytes
### getName() {#getName--}
```
public abstract String getName()
```


Obtiene el nombre de la entrada.

Archivos solo para compresión, como gzip, bzip2, lzip, lzma, xz, z, tienen el nombre "File.bin" a menos que se encuentre otro nombre en los encabezados.

**Returns:**
java.lang.String - el nombre de la entrada
