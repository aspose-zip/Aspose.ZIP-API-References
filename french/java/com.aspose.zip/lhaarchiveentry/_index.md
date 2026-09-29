---
title: "LhaArchiveEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans une archive Lha."
type: docs
weight: 76
url: /fr/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Représente un fichier unique dans une archive Lha.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrait l'entrée d'archive Lha vers un fichier. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée d'archive Lha vers le système de fichiers selon le chemin. |
| [getLastModified()](#getLastModified--) | Obtient la date de dernière modification de l'entrée. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getModificationTime()](#getModificationTime--) | Obtient la date de dernière modification de l'entrée. |
| [getName()](#getName--) | Obtient le nom de l'entrée. |
| [getPath()](#getPath--) | Obtient le chemin complet de l'entrée. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si cette entrée est un répertoire. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrait l'entrée d'archive Lha vers un fichier.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier qui stockera les données décompressées |

**Returns:**
java.io.File - instance java.io.File contenant les données extraites
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Obtient la date de dernière modification de l'entrée.

**Returns:**
java.util.Date - la date de dernière modification de l'entrée
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtient la date de dernière modification de l'entrée.

**Returns:**
java.util.Date - la date de dernière modification de l'entrée
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée.

Archives uniquement pour la compression, telles que gzip, bzip2, lzip, lzma, xz, z, ont le nom "File.bin" sauf si un autre nom peut être trouvé dans les en-têtes.

**Returns:**
java.lang.String - le nom de l'entrée
### getPath() {#getPath--}
```
public final String getPath()
```


Obtient le chemin complet de l'entrée.

**Returns:**
java.lang.String - le chemin complet de l'entrée
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtient une valeur indiquant si cette entrée est un répertoire.

**Returns:**
boolean - une valeur indiquant si cette entrée est un répertoire.
