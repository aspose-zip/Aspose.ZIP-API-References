---
title: "ArchiveInstanceInfo"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل معلومات حول نسخة الأرشيف."
type: docs
weight: 34
url: /ar/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

يمثل معلومات حول نسخة الأرشيف.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | يحصل على قيمة تشير إلى ما إذا كانت أسماء الإدخالات (الملفات) في الأرشيف مشفرة. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | يحصل على معلومات تنسيق الأرشيف. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | يحصل على معلومات تنسيق الأرشيف. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | يحصل على معلومات مثيل الأرشيف. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | يحصل على معلومات مثيل الأرشيف. |
| [getFormatInfo()](#getFormatInfo--) | يحصل على معلومات تنسيق الأرشيف. |
| [isContentEncrypted()](#isContentEncrypted--) | يحصل على قيمة تشير إلى ما إذا كان محتوى الأرشيف مشفرًا. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


يحصل على قيمة تشير إلى ما إذا كانت أسماء الإدخالات (الملفات) في الأرشيف مشفرة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت أسماء الإدخالات (الملفات) في الأرشيف مشفرة.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


يحصل على معلومات تنسيق الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | دفق ملف الأرشيف. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


يحصل على معلومات تنسيق الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


يحصل على معلومات مثيل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | دفق ملف الأرشيف. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


يحصل على معلومات مثيل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


يحصل على معلومات تنسيق الأرشيف.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


يحصل على قيمة تشير إلى ما إذا كان محتوى الأرشيف مشفرًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان محتوى الأرشيف مشفرًا.
