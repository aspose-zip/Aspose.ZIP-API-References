---
title: "ArchiveFormatDetector"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يكشف تنسيق الأرشيف ويقدم معلومات أخرى ذات صلة."
type: docs
weight: 32
url: /ar/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

يكشف تنسيق الأرشيف ويقدم معلومات أخرى ذات صلة.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | ينشئ مثيلاً جديدًا من الفئة [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | يحصل على معلومات التنسيق. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | يحصل على معلومات التنسيق. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


ينشئ مثيلاً جديدًا من الفئة [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


يحصل على معلومات التنسيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | دفق ملف الأرشيف. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


يحصل على معلومات التنسيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الأرشيف. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
