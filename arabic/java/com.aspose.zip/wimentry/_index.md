---
title: "WimEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا أو دليلًا واحدًا داخل صورة wim."
type: docs
weight: 132
url: /ar/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

تمثل ملفًا أو دليلًا واحدًا داخل صورة wim.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | يحصل على أسماء تدفقات البيانات البديلة للملف أو الدليل. |
| [getArchive()](#getArchive--) | يحصل على الأرشيف الذي ينتمي إليه العنصر. |
| [getChangeTime()](#getChangeTime--) | يحصل على آخر مرة تم فيها تغيير الملف أو الدليل. |
| [getCreationTime()](#getCreationTime--) | يحصل على وقت إنشاء الملف أو الدليل. |
| [getFileAttributes()](#getFileAttributes--) | يحصل على سمات الملف أو الدليل. |
| [getFullPath()](#getFullPath--) | يحصل على المسار الكامل للمدخل داخل الصورة. |
| [getHardLink()](#getHardLink--) | يحصل على معرف الارتباط الصلب للملف أو الدليل. |
| [getImage()](#getImage--) | يحصل على الصورة التي ينتمي إليها المدخل. |
| [getLastAccessTime()](#getLastAccessTime--) | يحصل على وقت الوصول الأخير للملف أو الدليل. |
| [getLastWriteTime()](#getLastWriteTime--) | يحصل على وقت التعديل للملف أو الدليل. |
| [getModificationTime()](#getModificationTime--) | يحصل على وقت التعديل للملف أو الدليل. |
| [getName()](#getName--) | يحصل على اسم الإدخال داخل الصورة. |
| [getParent()](#getParent--) | يحصل على الدليل الأب الذي ينتمي إليه الإدخال. |
| [getShortName()](#getShortName--) | يحصل على الاسم المختصر للإدخال داخل الصورة. |
| [hasHardLinks()](#hasHardLinks--) | يحصل على ما إذا كان الملف أو الدليل معروفًا بأسماء أخرى. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [toString()](#toString--) | يعيد تمثيل السلسلة للنسخة من الفئة [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


يحصل على أسماء تدفقات البيانات البديلة للملف أو الدليل.

**Returns:**
java.lang.String[] - أسماء تدفقات البيانات البديلة للملف أو الدليل
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


يحصل على الأرشيف الذي ينتمي إليه العنصر.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


يحصل على آخر مرة تم فيها تغيير الملف أو الدليل.

**Returns:**
java.util.Date - آخر مرة تم فيها تغيير الملف أو الدليل
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


يحصل على وقت إنشاء الملف أو الدليل.

**Returns:**
java.util.Date - وقت إنشاء الملف أو الدليل
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


يحصل على سمات الملف أو الدليل.

**Returns:**
int - سمات الملف أو الدليل
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


يحصل على المسار الكامل للمدخل داخل الصورة.

**Returns:**
java.lang.String - المسار الكامل للإدخال داخل الصورة
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


يحصل على معرف الارتباط الصلب للملف أو الدليل.

**Returns:**
long - معرف الارتباط الصلب للملف أو الدليل
### getImage() {#getImage--}
```
public final WimImage getImage()
```


يحصل على الصورة التي ينتمي إليها المدخل.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


يحصل على وقت الوصول الأخير للملف أو الدليل.

**Returns:**
java.util.Date - آخر وقت وصول للملف أو الدليل
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


يحصل على وقت التعديل للملف أو الدليل.

**Returns:**
java.util.Date - وقت تعديل الملف أو الدليل
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


يحصل على وقت التعديل للملف أو الدليل.

**Returns:**
java.util.Date - وقت تعديل الملف أو الدليل
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الإدخال داخل الصورة.

**Returns:**
java.lang.String - اسم الإدخال داخل الصورة
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


يحصل على الدليل الأب الذي ينتمي إليه الإدخال.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


يحصل على الاسم المختصر للإدخال داخل الصورة.

**Returns:**
java.lang.String - الاسم المختصر للإدخال داخل الصورة
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


يحصل على ما إذا كان الملف أو الدليل معروفًا بأسماء أخرى.

**Returns:**
boolean - ما إذا كان الملف أو الدليل معروفًا بأسماء أخرى
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا
### toString() {#toString--}
```
public String toString()
```


يعيد تمثيل السلسلة للنسخة من الفئة [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن
