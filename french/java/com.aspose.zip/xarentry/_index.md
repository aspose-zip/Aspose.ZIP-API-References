---
title: "XarEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente une seule entrée dans une archive xar."
type: docs
weight: 140
url: /fr/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Représente une seule entrée dans une archive xar.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Obtient la date de création du fichier ou du répertoire. |
| [getFullPath()](#getFullPath--) | Obtient le chemin complet de l'entrée dans l'archive. |
| [getLastAccessTime()](#getLastAccessTime--) | Obtient la dernière heure d'accès du fichier ou du répertoire. |
| [getLastWriteTime()](#getLastWriteTime--) | Obtient l'heure de modification du fichier ou du répertoire. |
| [getModificationTime()](#getModificationTime--) | Obtient l'heure de modification du fichier ou du répertoire. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getParent()](#getParent--) | Obtient le répertoire parent auquel l'entrée appartient. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne de l'instance de la classe [XarEntry](../../com.aspose.zip/xarentry). |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtient la date de création du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure de création du fichier ou du répertoire
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Obtient le chemin complet de l'entrée dans l'archive.

**Returns:**
java.lang.String - le chemin complet de l'entrée dans l'archive
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Obtient la dernière heure d'accès du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure du dernier accès au fichier ou au répertoire
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Obtient l'heure de modification du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure de modification du fichier ou du répertoire
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtient l'heure de modification du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure de modification du fichier ou du répertoire
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée dans l'archive.

**Returns:**
java.lang.String - le nom de l'entrée dans l'archive
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Obtient le répertoire parent auquel l'entrée appartient.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtient une valeur indiquant si l'entrée représente un répertoire.

**Returns:**
boolean - une valeur indiquant si l'entrée représente un répertoire
### toString() {#toString--}
```
public String toString()
```


Renvoie la représentation sous forme de chaîne de l'instance de la classe [XarEntry](../../com.aspose.zip/xarentry).

**Returns:**
java.lang.String - représentation sous forme de chaîne de cet objet
