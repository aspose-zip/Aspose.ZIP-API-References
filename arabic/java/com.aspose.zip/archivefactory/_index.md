---
title: "ArchiveFactory"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يكتشف تنسيق الأرشيف وينشئ الكائن المناسب وفقًا لنوع الأرشيف."
type: docs
weight: 31
url: /ar/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

يكتشف تنسيق الأرشيف وينشئ الكائن المناسب [IArchive](../../com.aspose.zip/iarchive) وفقًا لنوع الأرشيف.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | يضغط الدليل المحدد إلى ملف أرشيف باستخدام تنسيق الأرشيف المقدم. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | يكتشف تنسيق الأرشيف وينشئ الكائن المناسب [IArchive](../../com.aspose.zip/iarchive) وفقًا لنوع الأرشيف المحدد بواسطة الدفق المعطى. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | يكتشف تنسيق الأرشيف وينشئ الكائن المناسب [IArchive](../../com.aspose.zip/iarchive) وفقًا لنوع الأرشيف المشفر المحدد بواسطة الدفق المعطى. |
| [getArchive(String path)](#getArchive-java.lang.String-) | يكتشف تنسيق الأرشيف وينشئ الكائن المناسب [IArchive](../../com.aspose.zip/iarchive) وفقًا لنوع الأرشيف المحدد بواسطة المسار المعطى. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


يضغط الدليل المحدد إلى ملف أرشيف باستخدام تنسيق الأرشيف المقدم.

فيما يلي مثال على كيفية استخدام طريقة CompressDirectory:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// سيؤدي هذا إلى إنشاء ملف ZIP يحتوي على محتويات الدليل في المسار المحدد.
 
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
