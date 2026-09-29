---
title: "XarEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل إدخالًا واحدًا داخل أرشيف xar."
type: docs
weight: 140
url: /ar/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

تمثل إدخالًا واحدًا داخل أرشيف xar.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | يحصل على وقت إنشاء الملف أو الدليل. |
| [getFullPath()](#getFullPath--) | يحصل على المسار الكامل للمدخل داخل الأرشيف. |
| [getLastAccessTime()](#getLastAccessTime--) | يحصل على وقت الوصول الأخير للملف أو الدليل. |
| [getLastWriteTime()](#getLastWriteTime--) | يحصل على وقت التعديل للملف أو الدليل. |
| [getModificationTime()](#getModificationTime--) | يحصل على وقت التعديل للملف أو الدليل. |
| [getName()](#getName--) | يحصل على اسم العنصر داخل الأرشيف. |
| [getParent()](#getParent--) | يحصل على الدليل الأب الذي ينتمي إليه الإدخال. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [toString()](#toString--) | يعيد تمثيل النص لسلسلة كائن فئة [XarEntry](../../com.aspose.zip/xarentry). |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


يحصل على وقت إنشاء الملف أو الدليل.

**Returns:**
java.util.Date - وقت إنشاء الملف أو الدليل
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


يحصل على المسار الكامل للمدخل داخل الأرشيف.

**Returns:**
java.lang.String - المسار الكامل للمدخل داخل الأرشيف
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


يحصل على اسم العنصر داخل الأرشيف.

**Returns:**
java.lang.String - اسم العنصر داخل الأرشيف
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


يحصل على الدليل الأب الذي ينتمي إليه الإدخال.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


يعيد تمثيل النص لسلسلة كائن فئة [XarEntry](../../com.aspose.zip/xarentry).

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن
