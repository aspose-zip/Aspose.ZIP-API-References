---
title: "AppleArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa una entrada de archivo o directorio dentro de un ."
type: docs
weight: 17
url: /es/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Representa una entrada de archivo o directorio dentro de un [AppleArchive](../../com.aspose.zip/applearchive).

Una instancia de esta clase puede representar ya sea una entrada analizada de un Apple Archive existente o una entrada añadida a un archivo que se está componiendo.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada del archivo Apple a un sistema de archivos mediante la ruta. |
| [getLength()](#getLength--) | Obtiene la longitud descomprimida de la entrada en bytes. |
| [getName()](#getName--) | Obtiene la ruta de la entrada dentro del archivo. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino. Debe ser escribible |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae la entrada del archivo Apple a un sistema de archivos mediante la ruta.

```

``````

try (FileInputStream aaFile = new FileInputStream(\"archive.aa\")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
