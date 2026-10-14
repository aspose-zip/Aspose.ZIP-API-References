---
title: "AlzEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente une entrée de fichier dans une archive ALZ ainsi que ses métadonnées."
type: docs
weight: 13
url: /fr/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Représente une entrée de fichier dans une archive ALZ ainsi que ses métadonnées.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers un flux inscriptible. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrait l'entrée vers un flux inscriptible en utilisant un mot de passe optionnel. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le fichier spécifié. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrait l'entrée vers le fichier spécifié en utilisant un mot de passe optionnel. |
| [getCompressedSize()](#getCompressedSize--) | Obtient la taille compressée des données de l'entrée en octets. |
| [getLength()](#getLength--) | Obtient la longueur décompressée de cette entrée. |
| [getName()](#getName--) | Obtient le nom de l'entrée stocké dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille décompressée des données de l'entrée en octets. |
| [isDirectory()](#isDirectory--) | Obtient si cette entrée représente un répertoire. |
| [open()](#open--) | Ouvre l'entrée et fournit un flux contenant les données décompressées. |
| [open(String password)](#open-java.lang.String-) | Ouvre l'entrée et fournit un flux contenant les données décompressées. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers un flux inscriptible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extrait l'entrée vers un flux inscriptible en utilisant un mot de passe optionnel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination |
| password | java.lang.String | mot de passe optionnel pour cette entrée |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'entrée vers le fichier spécifié. Un fichier existant est écrasé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin du fichier de destination |

**Returns:**
java.io.File - fichier extrait
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extrait l'entrée vers le fichier spécifié en utilisant un mot de passe optionnel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin du fichier de destination |
| password | java.lang.String | mot de passe optionnel pour cette entrée |

**Returns:**
java.io.File - fichier extrait
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtient la taille compressée des données de l'entrée en octets.

**Returns:**
long - taille compressée en octets
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur décompressée de cette entrée.

**Returns:**
java.lang.Long - longueur non compressée en octets
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée stocké dans l'archive.

**Returns:**
java.lang.String - nom de l'entrée
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtient la taille décompressée des données de l'entrée en octets.

**Returns:**
long - taille non compressée en octets
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtient si cette entrée représente un répertoire.

**Returns:**
boolean - `true` pour une entrée de répertoire
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'entrée et fournit un flux contenant les données décompressées.

**Returns:**
java.io.InputStream - flux contenant les données de l'entrée décompressées
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Ouvre l'entrée et fournit un flux contenant les données décompressées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | mot de passe optionnel pour cette entrée |

**Returns:**
java.io.InputStream - flux contenant les données de l'entrée décompressées
