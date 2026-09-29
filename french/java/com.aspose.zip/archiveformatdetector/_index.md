---
title: "ArchiveFormatDetector"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Détecte un format d'archive et fournit d'autres informations connexes."
type: docs
weight: 32
url: /fr/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Détecte un format d'archive et fournit d'autres informations connexes.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Initialise une nouvelle instance de la classe [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Obtient les informations de format. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Obtient les informations de format. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Initialise une nouvelle instance de la classe [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Obtient les informations de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux du fichier d'archive. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Obtient les informations de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom de fichier du fichier d'archive. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
