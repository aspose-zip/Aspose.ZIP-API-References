---
title: "ArchiveFactory"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Détecte le format de l'archive et crée l'objet approprié selon le type d'archive."
type: docs
weight: 31
url: /fr/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Détecte le format de l'archive et crée l'objet [IArchive](../../com.aspose.zip/iarchive) approprié selon le type d'archive.
## Méthodes

| Méthode | Description |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Compresse le répertoire spécifié dans un fichier d'archive en utilisant le format d'archive fourni. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Détecte le format de l'archive et crée l'objet [IArchive](../../com.aspose.zip/iarchive) approprié selon le type d'archive spécifié par le flux fourni. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Détecte le format de l'archive et crée l'objet [IArchive](../../com.aspose.zip/iarchive) approprié selon le type d'archive chiffrée spécifié par le flux fourni. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Détecte le format de l'archive et crée l'objet [IArchive](../../com.aspose.zip/iarchive) approprié selon le type d'archive spécifié par le chemin fourni. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Compresse le répertoire spécifié dans un fichier d'archive en utilisant le format d'archive fourni.

Voici un exemple d'utilisation de la méthode CompressDirectory :

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Cela créera un fichier ZIP contenant le contenu du répertoire au chemin spécifié.
 
```

This method will create an archive file at the location specified by the `path` parameter. The name of the archive file will typically be the directory name followed by the appropriate file extension based on the `archiveFormat`. The directory itself is not modified or deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the directory that will be compressed |
| outputFileName | java.lang.String | destination file name |
| archiveFormat | [ArchiveFormat](../../com.aspose.zip/archiveformat) | the format of the archive to create (e.g., zip, rar, tar, etc.) |

### getArchive(InputStream stream) {#getArchive-java.io.InputStream-}
```
public static IArchive getArchive(InputStream stream)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(InputStream stream, String password) {#getArchive-java.io.InputStream-java.lang.String-}
```
public static IArchive getArchive(InputStream stream, String password)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of encrypted archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |
| password | java.lang.String | password to decrypt an encrypted archive |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(String path) {#getArchive-java.lang.String-}
```
public static IArchive getArchive(String path)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive to be analyzed |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
