---
title: ComHelper
second_title: Aspose.ZIP for Java API Reference
description: Provides methods for COM clients to load archives into Aspose.Zip.
type: docs
weight: 40
url: /java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Provides methods for COM clients to load archives into Aspose.Zip.

Use the ComHelper class to load an archive from a file or stream. Particular classes provide a default constructor to create a new archive and also provides overloaded constructors to load an archive from a file or stream. If you are using Aspose.Zip from a .NET application, you can use all the archive constructors directly, but if you are using Aspose.Zip from a COM application, only the default archive constructor is available.
## Constructors

| Constructor | Description |
| --- | --- |
| [ComHelper()](#ComHelper--) | Initializes a new instance of this class. |
## Methods

| Method | Description |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Allows a COM application to load a bzip2 archive from a stream. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Allows a COM application to load a bzip2 archive from a file. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Allows a COM application to load a gzip archive from a stream. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Allows a COM application to load a gzip archive from a file. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Allows a COM application to load a rar archive from a stream. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Allows a COM application to load a rar archive from a file. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Allows a COM application to load a ZIP archive from a stream. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Allows a COM application to load a ZIP archive from a file. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Initializes a new instance of this class.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Allows a COM application to load a bzip2 archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A .NET stream object that contains the archive to load. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Allows a COM application to load a bzip2 archive from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Filename of the archive to load. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Allows a COM application to load a gzip archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A .NET stream object that contains the archive to load. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Allows a COM application to load a gzip archive from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Filename of the archive to load. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Allows a COM application to load a rar archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A .NET stream object that contains the archive to load. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Allows a COM application to load a rar archive from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Filename of the archive to load. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Allows a COM application to load a ZIP archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A .NET stream object that contains the archive to load. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Allows a COM application to load a ZIP archive from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Filename of the archive to load. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
