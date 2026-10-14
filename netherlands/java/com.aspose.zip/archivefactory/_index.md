---
title: "ArchiveFactory"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Detecteert het archiefformaat en maakt het juiste object aan volgens het type archief."
type: docs
weight: 31
url: /nl/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Detecteert het archiefformaat en maakt het juiste [IArchive](../../com.aspose.zip/iarchive) object aan volgens het type archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Comprimeert de opgegeven map naar een archiefbestand met behulp van het opgegeven archiefformaat. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Detecteert het archiefformaat en maakt het juiste [IArchive](../../com.aspose.zip/iarchive) object aan volgens het type archief dat is opgegeven door de gegeven stream. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Detecteert het archiefformaat en maakt het juiste [IArchive](../../com.aspose.zip/iarchive) object aan volgens het type versleuteld archief dat is opgegeven door de gegeven stream. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Detecteert het archiefformaat en maakt het juiste [IArchive](../../com.aspose.zip/iarchive) object aan volgens het type archief dat is opgegeven door het gegeven pad. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Comprimeert de opgegeven map naar een archiefbestand met behulp van het opgegeven archiefformaat.

Hier is een voorbeeld van hoe de methode CompressDirectory te gebruiken:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Dit maakt een ZIP-bestand aan met de inhoud van de map op het opgegeven pad.
 
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
