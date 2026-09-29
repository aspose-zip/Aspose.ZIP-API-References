---
title: "ComHelper"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Fournit des méthodes pour les clients COM afin de charger des archives dans Aspose.Zip."
type: docs
weight: 55
url: /fr/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Fournit des méthodes pour les clients COM afin de charger des archives dans Aspose.Zip.

Utilisez la classe ComHelper pour charger une archive à partir d'un fichier ou d'un flux. Certaines classes offrent un constructeur par défaut pour créer une nouvelle archive et fournissent également des constructeurs surchargés pour charger une archive à partir d'un fichier ou d'un flux. Si vous utilisez Aspose.Zip depuis une application .NET, vous pouvez utiliser tous les constructeurs d'archive directement, mais si vous utilisez Aspose.Zip depuis une application COM, seul le constructeur d'archive par défaut est disponible.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ComHelper()](#ComHelper--) | Initialise une nouvelle instance de cette classe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Permet à une application COM de charger une archive bzip2 depuis un flux. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Permet à une application COM de charger une archive bzip2 depuis un fichier. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Permet à une application COM de charger une archive gzip depuis un flux. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Permet à une application COM de charger une archive gzip depuis un fichier. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Permet à une application COM de charger une archive rar depuis un flux. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Permet à une application COM de charger une archive rar depuis un fichier. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Permet à une application COM de charger une archive ZIP depuis un flux. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Permet à une application COM de charger une archive ZIP depuis un fichier. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Initialise une nouvelle instance de cette classe.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Permet à une application COM de charger une archive bzip2 depuis un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Un objet flux .NET qui contient l'archive à charger. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Permet à une application COM de charger une archive bzip2 depuis un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Nom de fichier de l'archive à charger. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Permet à une application COM de charger une archive gzip depuis un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Un objet flux .NET qui contient l'archive à charger. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Permet à une application COM de charger une archive gzip depuis un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Nom de fichier de l'archive à charger. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Permet à une application COM de charger une archive rar depuis un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Un objet flux .NET qui contient l'archive à charger. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Permet à une application COM de charger une archive rar depuis un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Nom de fichier de l'archive à charger. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Permet à une application COM de charger une archive ZIP depuis un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Un objet flux .NET qui contient l'archive à charger. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Permet à une application COM de charger une archive ZIP depuis un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Nom de fichier de l'archive à charger. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
