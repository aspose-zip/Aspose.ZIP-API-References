---
title: "AppleArchiveEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente une entrée de fichier ou de répertoire dans un."
type: docs
weight: 17
url: /fr/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Représente une entrée de fichier ou de répertoire dans un [AppleArchive](../../com.aspose.zip/applearchive).

Une instance de cette classe peut représenter soit une entrée analysée à partir d'une Apple Archive existante, soit une entrée ajoutée à une archive en cours de composition.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée d'archive Apple vers un système de fichiers par chemin. |
| [getLength()](#getLength--) | Obtient la longueur non compressée de l'entrée en octets. |
| [getName()](#getName--) | Obtient le chemin de l'entrée à l'intérieur de l'archive. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination. Doit être accessible en écriture |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'entrée d'archive Apple vers un système de fichiers par chemin.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
