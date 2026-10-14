---
title: "LzxArchiveEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans une archive LZX."
type: docs
weight: 90
url: /fr/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Représente un fichier unique dans une archive LZX.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée d'archive Lzx vers un système de fichiers par chemin. |
| [getCommentary()](#getCommentary--) | Obtient le commentaire. |
| [getCompressedSize()](#getCompressedSize--) | Obtient la taille du fichier compressé. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getModificationTime()](#getModificationTime--) | Obtient la date de dernière modification de l'entrée. |
| [getName()](#getName--) | Obtient le nom de l'entrée. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille du fichier original. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si cette entrée est un répertoire. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Flux de destination. Doit être accessible en écriture. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'entrée d'archive Lzx vers un système de fichiers par chemin.

```

``````

try (FileInputStream lzxFile = new FileInputStream(\"archive.lzx\")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
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
