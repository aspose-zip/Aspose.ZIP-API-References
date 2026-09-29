---
title: "ArjEntryPlain"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo ARJ."
type: docs
weight: 38
url: /es/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo ARJ.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrae la entrada del archivo ARJ a un archivo. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño del archivo comprimido. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño del archivo original. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrae la entrada del archivo ARJ a un archivo.

```

``````

try (FileInputStream arjFile = new FileInputStream(\"sourceFileName\")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

**Returns:**
java.io.File - la información del archivo compuesto
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtiene el tamaño del archivo comprimido.

**Returns:**
long - el tamaño del archivo comprimido
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtiene la longitud de la entrada en bytes.

**Returns:**
java.lang.Long - la longitud de la entrada en bytes
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada dentro del archivo.

**Returns:**
java.lang.String - nombre de la entrada dentro del archivo
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtiene el tamaño del archivo original.

**Returns:**
long - tamaño del archivo original
