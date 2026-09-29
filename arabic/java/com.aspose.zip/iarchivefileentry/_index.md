---
title: "IArchiveFileEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الواجهة تمثل مدخل ملف أرشيف."
type: docs
weight: 162
url: /ar/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

هذه الواجهة تمثل مدخل ملف أرشيف.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getName()](#getName--) | يحصل على اسم الإدخال. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة. يجب أن يكون قابلًا للكتابة |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


يستخرج المدخل إلى نظام الملفات بالمسار المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - كائن java.io.File يحتوي على البيانات المستخرجة
### getLength() {#getLength--}
```
public abstract Long getLength()
```


يحصل على طول المدخل بالبايت.

**Returns:**
java.lang.Long - طول الإدخال بالبايت
### getName() {#getName--}
```
public abstract String getName()
```


يحصل على اسم الإدخال.

الأرشيفات للضغط فقط، مثل gzip و bzip2 و lzip و lzma و xz و z لها الاسم "File.bin" ما لم يتم العثور على اسم آخر في رؤوس الملفات.

**Returns:**
java.lang.String - اسم الإدخال
