---
title: "ArjEntryPlain"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans une archive ARJ."
type: docs
weight: 38
url: /fr/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Représente un fichier unique dans une archive ARJ.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrait une entrée d'archive ARJ vers un fichier. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getCompressedSize()](#getCompressedSize--) | Obtient la taille du fichier compressé. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille du fichier original. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrait une entrée d'archive ARJ vers un fichier.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - les informations du fichier composé
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtient la taille du fichier compressé.

**Returns:**
long - la taille du fichier compressé
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée dans l'archive.

**Returns:**
java.lang.String - nom de l'entrée dans l'archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtient la taille du fichier original.

**Returns:**
long - taille du fichier original
