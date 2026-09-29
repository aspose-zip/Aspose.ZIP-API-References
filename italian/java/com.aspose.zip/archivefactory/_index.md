---
title: "ArchiveFactory"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rileva il formato dell'archivio e crea l'oggetto appropriato in base al tipo di archivio."
type: docs
weight: 31
url: /it/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Rileva il formato dell'archivio e crea l'oggetto [IArchive](../../com.aspose.zip/iarchive) appropriato in base al tipo di archivio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Comprimi la directory specificata in un file di archivio utilizzando il formato di archivio fornito. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Rileva il formato dell'archivio e crea l'oggetto [IArchive](../../com.aspose.zip/iarchive) appropriato in base al tipo di archivio specificato dallo stream fornito. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Rileva il formato dell'archivio e crea l'oggetto [IArchive](../../com.aspose.zip/iarchive) appropriato in base al tipo di archivio crittografato specificato dallo stream fornito. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Rileva il formato dell'archivio e crea l'oggetto [IArchive](../../com.aspose.zip/iarchive) appropriato in base al tipo di archivio specificato dal percorso fornito. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Comprimi la directory specificata in un file di archivio utilizzando il formato di archivio fornito.

Ecco un esempio di come utilizzare il metodo CompressDirectory:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Questo creerà un file ZIP con il contenuto della directory al percorso specificato.
 
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
