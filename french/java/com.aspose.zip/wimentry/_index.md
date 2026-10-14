---
title: "WimEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un seul fichier ou répertoire dans une image wim."
type: docs
weight: 132
url: /fr/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Représente un seul fichier ou répertoire dans une image wim.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Obtient les noms des flux de données alternatifs du fichier ou du répertoire. |
| [getArchive()](#getArchive--) | Obtient l'archive à laquelle l'entrée appartient. |
| [getChangeTime()](#getChangeTime--) | Obtient la dernière fois que le fichier ou le répertoire a été modifié. |
| [getCreationTime()](#getCreationTime--) | Obtient la date de création du fichier ou du répertoire. |
| [getFileAttributes()](#getFileAttributes--) | Obtient les attributs du fichier ou du répertoire. |
| [getFullPath()](#getFullPath--) | Obtient le chemin complet de l'entrée dans l'image. |
| [getHardLink()](#getHardLink--) | Obtient l'identifiant du lien physique du fichier ou du répertoire. |
| [getImage()](#getImage--) | Obtient l'image à laquelle l'entrée appartient. |
| [getLastAccessTime()](#getLastAccessTime--) | Obtient la dernière heure d'accès du fichier ou du répertoire. |
| [getLastWriteTime()](#getLastWriteTime--) | Obtient l'heure de modification du fichier ou du répertoire. |
| [getModificationTime()](#getModificationTime--) | Obtient l'heure de modification du fichier ou du répertoire. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'image. |
| [getParent()](#getParent--) | Obtient le répertoire parent auquel l'entrée appartient. |
| [getShortName()](#getShortName--) | Obtient le nom court de l'entrée dans l'image. |
| [hasHardLinks()](#hasHardLinks--) | Obtient si le fichier ou le répertoire est connu sous d'autres noms. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne de l'instance de la classe [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Obtient les noms des flux de données alternatifs du fichier ou du répertoire.

**Returns:**
java.lang.String[] - les noms des flux de données alternatifs du fichier ou du répertoire
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Obtient l'archive à laquelle l'entrée appartient.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Obtient la dernière fois que le fichier ou le répertoire a été modifié.

**Returns:**
java.util.Date - la dernière fois que le fichier ou le répertoire a été modifié
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtient la date de création du fichier ou du répertoire.

**Returns:**
java.util.Date - l'heure de création du fichier ou du répertoire
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Obtient les attributs du fichier ou du répertoire.

**Returns:**
int - les attributs du fichier ou du répertoire
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Obtient le chemin complet de l'entrée dans l'image.

**Returns:**
java.lang.String - le chemin complet de l'entrée dans l'image
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Obtient l'identifiant du lien physique du fichier ou du répertoire.

**Returns:**
long - l'identifiant du lien dur du fichier ou du répertoire
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Obtient l'image à laquelle l'entrée appartient.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
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


Obtient le nom de l'entrée dans l'image.

**Returns:**
java.lang.String - le nom de l'entrée dans l'image
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Obtient le répertoire parent auquel l'entrée appartient.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Obtient le nom court de l'entrée dans l'image.

**Returns:**
java.lang.String - le nom court de l'entrée dans l'image
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Obtient si le fichier ou le répertoire est connu sous d'autres noms.

**Returns:**
boolean - si le fichier ou le répertoire est connu sous d'autres noms
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


Renvoie la représentation sous forme de chaîne de l'instance de la classe [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - représentation sous forme de chaîne de cet objet
