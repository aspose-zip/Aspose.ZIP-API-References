---
title: "ArchiveFactory"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Erkennt das Archivformat und erstellt das entsprechende Objekt gemäß dem Typ des Archivs."
type: docs
weight: 31
url: /de/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Erkennt das Archivformat und erstellt das entsprechende [IArchive](../../com.aspose.zip/iarchive)-Objekt gemäß dem Typ des Archivs.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Komprimiert das angegebene Verzeichnis in eine Archivdatei unter Verwendung des bereitgestellten Archivformats. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Erkennt das Archivformat und erstellt das entsprechende [IArchive](../../com.aspose.zip/iarchive)-Objekt gemäß dem Typ des Archivs, der durch den angegebenen Stream bestimmt wird. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Erkennt das Archivformat und erstellt das entsprechende [IArchive](../../com.aspose.zip/iarchive)-Objekt gemäß dem Typ des verschlüsselten Archivs, der durch den angegebenen Stream bestimmt wird. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Erkennt das Archivformat und erstellt das entsprechende [IArchive](../../com.aspose.zip/iarchive)-Objekt gemäß dem Typ des Archivs, der durch den angegebenen Pfad bestimmt wird. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Komprimiert das angegebene Verzeichnis in eine Archivdatei unter Verwendung des bereitgestellten Archivformats.

Hier ist ein Beispiel, wie die Methode CompressDirectory verwendet wird:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Dies erstellt eine ZIP-Datei mit dem Inhalt des Verzeichnisses am angegebenen Pfad.
 
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
