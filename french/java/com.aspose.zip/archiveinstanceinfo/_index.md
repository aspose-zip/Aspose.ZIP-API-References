---
title: "ArchiveInstanceInfo"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente les informations sur l'instance de l'archive."
type: docs
weight: 34
url: /fr/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Représente les informations sur l'instance de l'archive.
## Méthodes

| Méthode | Description |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Obtient une valeur indiquant si les noms des entrées (fichiers) de l'archive sont chiffrés. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Obtient les informations du format d'archive. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Obtient les informations du format d'archive. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Obtient les informations de l'instance d'archive. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Obtient les informations de l'instance d'archive. |
| [getFormatInfo()](#getFormatInfo--) | Obtient les informations du format d'archive. |
| [isContentEncrypted()](#isContentEncrypted--) | Obtient une valeur indiquant si le contenu de l'archive est chiffré. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Obtient une valeur indiquant si les noms des entrées (fichiers) de l'archive sont chiffrés.

**Returns:**
boolean - une valeur indiquant si les noms des entrées (fichiers) de l'archive sont chiffrés.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Obtient les informations du format d'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux du fichier d'archive. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Obtient les informations du format d'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom de fichier du fichier d'archive. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Obtient les informations de l'instance d'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux du fichier d'archive. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Obtient les informations de l'instance d'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom de fichier du fichier d'archive. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Obtient les informations du format d'archive.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Obtient une valeur indiquant si le contenu de l'archive est chiffré.

**Returns:**
boolean - une valeur indiquant si le contenu de l'archive est chiffré.
