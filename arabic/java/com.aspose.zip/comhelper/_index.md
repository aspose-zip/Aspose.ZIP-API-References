---
title: "ComHelper"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يوفر طرقًا لعملاء COM لتحميل الأرشيفات إلى Aspose.Zip."
type: docs
weight: 55
url: /ar/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

يوفر طرقًا لعملاء COM لتحميل الأرشيفات إلى Aspose.Zip.

استخدم فئة ComHelper لتحميل أرشيف من ملف أو تدفق. توفر الفئات المحددة مُنشئًا افتراضيًا لإنشاء أرشيف جديد وتوفر أيضًا مُنشئات مُحمَّلة لتحميل أرشيف من ملف أو تدفق. إذا كنت تستخدم Aspose.Zip من تطبيق .NET، يمكنك استخدام جميع مُنشئات الأرشيف مباشرةً، ولكن إذا كنت تستخدم Aspose.Zip من تطبيق COM، فإن مُنشئ الأرشيف الافتراضي فقط هو المتاح.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ComHelper()](#ComHelper--) | يُنشئ مثيلًا جديدًا من هذه الفئة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | يسمح لتطبيق COM بتحميل أرشيف bzip2 من تدفق. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | يسمح لتطبيق COM بتحميل أرشيف bzip2 من ملف. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | يسمح لتطبيق COM بتحميل أرشيف gzip من تدفق. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | يسمح لتطبيق COM بتحميل أرشيف gzip من ملف. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | يسمح لتطبيق COM بتحميل أرشيف rar من تدفق. |
| [openRar(String fileName)](#openRar-java.lang.String-) | يسمح لتطبيق COM بتحميل أرشيف rar من ملف. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | يسمح لتطبيق COM بتحميل أرشيف ZIP من تدفق. |
| [openZip(String fileName)](#openZip-java.lang.String-) | يسمح لتطبيق COM بتحميل أرشيف ZIP من ملف. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


يُنشئ مثيلًا جديدًا من هذه الفئة.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


يسمح لتطبيق COM بتحميل أرشيف bzip2 من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | كائن تدفق .NET يحتوي على الأرشيف المراد تحميله. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


يسمح لتطبيق COM بتحميل أرشيف bzip2 من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف المراد تحميله. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


يسمح لتطبيق COM بتحميل أرشيف gzip من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | كائن تدفق .NET يحتوي على الأرشيف المراد تحميله. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


يسمح لتطبيق COM بتحميل أرشيف gzip من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف المراد تحميله. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


يسمح لتطبيق COM بتحميل أرشيف rar من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | كائن تدفق .NET يحتوي على الأرشيف المراد تحميله. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


يسمح لتطبيق COM بتحميل أرشيف rar من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف المراد تحميله. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


يسمح لتطبيق COM بتحميل أرشيف ZIP من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | كائن تدفق .NET يحتوي على الأرشيف المراد تحميله. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


يسمح لتطبيق COM بتحميل أرشيف ZIP من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف المراد تحميله. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
