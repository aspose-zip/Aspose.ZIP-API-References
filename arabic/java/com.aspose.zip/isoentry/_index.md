---
title: "IsoEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل ملف إدخال أو دليل داخل أرشيف ISO."
type: docs
weight: 72
url: /ar/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

تمثل مدخلاً (ملف أو دليل) داخل أرشيف ISO.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getLength()](#getLength--) | يحصل على طول الإدخال. |
| [getModificationTime()](#getModificationTime--) | يحصل على تاريخ ووقت التعديل الأخير. |
| [getName()](#getName--) | يحصل على اسم الإدخال. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال دليلًا. |
| [toString()](#toString--) | يرجع سلسلة تمثل الإدخال الحالي. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


يستخرج المدخل إلى نظام الملفات بالمسار المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |

**Returns:**
java.io.File - كائن java.io.File يحتوي على البيانات المستخرجة
### getLength() {#getLength--}
```
public Long getLength()
```


يحصل على طول الإدخال.

**Returns:**
java.lang.Long - طول الإدخال
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


يحصل على تاريخ ووقت التعديل الأخير.

**Returns:**
java.util.Date - تاريخ ووقت التعديل الأخير
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الإدخال.

**Returns:**
java.lang.String - اسم الإدخال
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على قيمة تشير إلى ما إذا كان الإدخال دليلًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا
### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل الإدخال الحالي.

**Returns:**
java.lang.String - اسم الإدخال
