---
title: "LhaArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف Lha."
type: docs
weight: 76
url: /ar/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف Lha.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | يستخرج إدخال أرشيف Lha إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج إدخال أرشيف Lha إلى نظام ملفات حسب المسار. |
| [getLastModified()](#getLastModified--) | يحصل على وقت التعديل الأخير للإدخال. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getModificationTime()](#getModificationTime--) | يحصل على وقت التعديل الأخير للإدخال. |
| [getName()](#getName--) | يحصل على اسم الإدخال. |
| [getPath()](#getPath--) | يحصل على المسار الكامل للإدخال. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان هذا الإدخال مجلدًا. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


يستخرج إدخال أرشيف Lha إلى ملف.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى الملف الذي سيخزن البيانات غير المضغوطة |

**Returns:**
java.io.File - كائن java.io.File يحتوي على البيانات المستخرجة
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


يحصل على وقت التعديل الأخير للإدخال.

**Returns:**
java.util.Date - وقت التعديل الأخير للعنصر
### getLength() {#getLength--}
```
public final Long getLength()
```


يحصل على طول المدخل بالبايت.

**Returns:**
java.lang.Long - طول الإدخال بالبايت
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


يحصل على وقت التعديل الأخير للإدخال.

**Returns:**
java.util.Date - وقت التعديل الأخير للعنصر
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الإدخال.

الأرشيفات للضغط فقط، مثل gzip و bzip2 و lzip و lzma و xz و z لها الاسم "File.bin" ما لم يتم العثور على اسم آخر في رؤوس الملفات.

**Returns:**
java.lang.String - اسم الإدخال
### getPath() {#getPath--}
```
public final String getPath()
```


يحصل على المسار الكامل للإدخال.

**Returns:**
java.lang.String - المسار الكامل للعنصر
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على قيمة تشير إلى ما إذا كان هذا الإدخال مجلدًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان هذا العنصر دليلًا.
