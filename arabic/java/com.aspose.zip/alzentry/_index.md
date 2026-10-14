---
title: "AlzEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل إدخال ملف في أرشيف ALZ مع بياناته الوصفية."
type: docs
weight: 13
url: /ar/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

يمثل إدخال ملف في أرشيف ALZ مع بياناته الوصفية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى دفق قابل للكتابة. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | يستخرج المدخل إلى دفق قابل للكتابة باستخدام كلمة مرور اختيارية. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى الملف المحدد. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | يستخرج المدخل إلى الملف المحدد باستخدام كلمة مرور اختيارية. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على الحجم المضغوط لبيانات المدخل بالبايت. |
| [getLength()](#getLength--) | يحصل على الطول غير المضغوط لهذا الإدخال. |
| [getName()](#getName--) | يحصل على اسم الإدخال المخزن في الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على الحجم غير المضغوط لبيانات الإدخال بالبايت. |
| [isDirectory()](#isDirectory--) | يحصل على ما إذا كان هذا الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح الإدخال ويوفر تدفقًا يحتوي على البيانات غير المضغوطة. |
| [open(String password)](#open-java.lang.String-) | يفتح الإدخال ويوفر تدفقًا يحتوي على البيانات غير المضغوطة. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى دفق قابل للكتابة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


يستخرج المدخل إلى دفق قابل للكتابة باستخدام كلمة مرور اختيارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لهذا الإدخال |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج الإدخال إلى الملف المحدد. يتم استبدال ملف موجود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الوجهة |

**Returns:**
java.io.File - ملف مستخرج
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


يستخرج المدخل إلى الملف المحدد باستخدام كلمة مرور اختيارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الوجهة |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لهذا الإدخال |

**Returns:**
java.io.File - ملف مستخرج
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


يحصل على الحجم المضغوط لبيانات المدخل بالبايت.

**Returns:**
long - الحجم المضغوط بالبايت
### getLength() {#getLength--}
```
public final Long getLength()
```


يحصل على الطول غير المضغوط لهذا الإدخال.

**Returns:**
java.lang.Long - الطول غير المضغوط بالبايت
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الإدخال المخزن في الأرشيف.

**Returns:**
java.lang.String - اسم الإدخال
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


يحصل على الحجم غير المضغوط لبيانات الإدخال بالبايت.

**Returns:**
long - الحجم غير المضغوط بالبايت
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على ما إذا كان هذا الإدخال يمثل دليلًا.

**Returns:**
boolean - `true` لإدخال دليل
### open() {#open--}
```
public final InputStream open()
```


يفتح الإدخال ويوفر تدفقًا يحتوي على البيانات غير المضغوطة.

**Returns:**
java.io.InputStream - تدفق يحتوي على بيانات الإدخال غير المضغوطة
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


يفتح الإدخال ويوفر تدفقًا يحتوي على البيانات غير المضغوطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لهذا الإدخال |

**Returns:**
java.io.InputStream - تدفق يحتوي على بيانات الإدخال غير المضغوطة
