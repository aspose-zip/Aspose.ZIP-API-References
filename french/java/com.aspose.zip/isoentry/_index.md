---
title: "IsoEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier ou un répertoire d'entrée dans une archive ISO."
type: docs
weight: 72
url: /fr/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Représente une entrée (fichier ou répertoire) dans une archive ISO.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée. |
| [getModificationTime()](#getModificationTime--) | Obtient la date et l'heure de dernière modification. |
| [getName()](#getName--) | Obtient le nom de l'entrée. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée est un répertoire. |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'entrée actuelle. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé |

**Returns:**
java.io.File - instance java.io.File contenant les données extraites
### getLength() {#getLength--}
```
public Long getLength()
```


Obtient la longueur de l'entrée.

**Returns:**
java.lang.Long - la longueur de l'entrée
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtient la date et l'heure de dernière modification.

**Returns:**
java.util.Date - date et heure de dernière modification
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée.

**Returns:**
java.lang.String - le nom de l'entrée
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtient une valeur indiquant si l'entrée est un répertoire.

**Returns:**
boolean - une valeur indiquant si l'entrée représente un répertoire
### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'entrée actuelle.

**Returns:**
java.lang.String - le nom de l'entrée
