---
title: "LhaArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo Lha."
type: docs
weight: 76
url: /es/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo Lha.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrae la entrada del archivo Lha a un archivo. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada del archivo Lha a un sistema de archivos por ruta. |
| [getLastModified()](#getLastModified--) | Obtiene la hora de última modificación de la entrada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getModificationTime()](#getModificationTime--) | Obtiene la hora de última modificación de la entrada. |
| [getName()](#getName--) | Obtiene el nombre de la entrada. |
| [getPath()](#getPath--) | Obtiene la ruta completa de la entrada. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si esta entrada es un directorio. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrae la entrada del archivo Lha a un archivo.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo que almacenará los datos descomprimidos |

**Returns:**
java.io.File - instancia de java.io.File que contiene los datos extraídos
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Obtiene la hora de última modificación de la entrada.

**Returns:**
java.util.Date - la hora de última modificación de la entrada
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtiene la longitud de la entrada en bytes.

**Returns:**
java.lang.Long - la longitud de la entrada en bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtiene la hora de última modificación de la entrada.

**Returns:**
java.util.Date - la hora de última modificación de la entrada
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada.

Archivos solo para compresión, como gzip, bzip2, lzip, lzma, xz, z, tienen el nombre "File.bin" a menos que se encuentre otro nombre en los encabezados.

**Returns:**
java.lang.String - el nombre de la entrada
### getPath() {#getPath--}
```
public final String getPath()
```


Obtiene la ruta completa de la entrada.

**Returns:**
java.lang.String - la ruta completa de la entrada
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtiene un valor que indica si esta entrada es un directorio.

**Returns:**
boolean - un valor que indica si esta entrada es un directorio.
