---
title: "IArchiveFileEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette interface représente une entrée de fichier d'archive."
type: docs
weight: 162
url: /fr/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Cette interface représente une entrée de fichier d'archive.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getName()](#getName--) | Obtient le nom de l'entrée. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination. Doit être accessible en écriture |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - instance java.io.File contenant les données extraites
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### getName() {#getName--}
```
public abstract String getName()
```


Obtient le nom de l'entrée.

Archives uniquement pour la compression, telles que gzip, bzip2, lzip, lzma, xz, z, ont le nom "File.bin" sauf si un autre nom peut être trouvé dans les en-têtes.

**Returns:**
java.lang.String - le nom de l'entrée
