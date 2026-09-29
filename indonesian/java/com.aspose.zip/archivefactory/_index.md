---
title: "ArchiveFactory"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mendeteksi format arsip dan membuat objek yang sesuai menurut jenis arsip."
type: docs
weight: 31
url: /id/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Mendeteksi format arsip dan membuat objek [IArchive](../../com.aspose.zip/iarchive) yang sesuai menurut jenis arsip.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Mengompres direktori yang ditentukan menjadi file arsip menggunakan format arsip yang disediakan. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Mendeteksi format arsip dan membuat objek [IArchive](../../com.aspose.zip/iarchive) yang sesuai menurut jenis arsip yang ditentukan oleh aliran yang diberikan. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Mendeteksi format arsip dan membuat objek [IArchive](../../com.aspose.zip/iarchive) yang sesuai menurut jenis arsip terenkripsi yang ditentukan oleh aliran yang diberikan. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Mendeteksi format arsip dan membuat objek [IArchive](../../com.aspose.zip/iarchive) yang sesuai menurut jenis arsip yang ditentukan oleh jalur yang diberikan. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Mengompres direktori yang ditentukan menjadi file arsip menggunakan format arsip yang disediakan.

Berikut contoh cara menggunakan metode CompressDirectory:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Ini akan membuat file ZIP dengan isi direktori pada jalur yang ditentukan.
 
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
