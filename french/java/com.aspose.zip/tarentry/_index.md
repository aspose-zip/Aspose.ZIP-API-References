---
title: "TarEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans une archive tar."
type: docs
weight: 126
url: /fr/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Représente un fichier unique dans une archive tar.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getModificationTime()](#getModificationTime--) | Obtient l'heure de modification du fichier ou du répertoire. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille d'un fichier original. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de l'entrée dans l'archive. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

Extrait une entrée d'une archive tar.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - les informations du fichier extrait
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


Obtient l'heure de modification du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure de modification du fichier ou du répertoire.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée dans l'archive.

**Returns:**
java.lang.String - le nom de l'entrée dans l'archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtient la taille d'un fichier original.

A la même valeur que `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - la taille d'un fichier original.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtient une valeur indiquant si l'entrée représente un répertoire.

**Returns:**
boolean - une valeur indiquant si l'entrée représente un répertoire
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée.


Utilisation :

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

