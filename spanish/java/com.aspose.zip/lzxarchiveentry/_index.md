---
title: "LzxArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo LZX."
type: docs
weight: 90
url: /es/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo LZX.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada del archivo Lzx a un sistema de archivos por ruta. |
| [getCommentary()](#getCommentary--) | Obtiene el comentario. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño del archivo comprimido. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getModificationTime()](#getModificationTime--) | Obtiene la hora de última modificación de la entrada. |
| [getName()](#getName--) | Obtiene el nombre de la entrada. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño del archivo original. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si esta entrada es un directorio. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | Flujo de destino. Debe ser escribible. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae la entrada del archivo Lzx a un sistema de archivos por ruta.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
