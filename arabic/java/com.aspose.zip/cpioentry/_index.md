---
title: "CpioEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف cpio."
type: docs
weight: 58
url: /ar/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف cpio.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | يحصل على وقت الكتابة الأخير. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getName()](#getName--) | يحصل على اسم العنصر داخل الأرشيف. |
| [getParent()](#getParent--) | يحصل على الأرشيف الذي ينتمي إليه العنصر. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
| [toString()](#toString--) | يعيد تمثيل السلسلة للنسخة من فئة [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخراج عنصر من أرشيف cpio.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف المستخرج
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


يحصل على وقت الكتابة الأخير.

**Returns:**
java.util.Date - وقت الكتابة الأخير
### getLength() {#getLength--}
```
public final Long getLength()
```


يحصل على طول المدخل بالبايت.

**Returns:**
java.lang.Long - طول الإدخال بالبايت
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم العنصر داخل الأرشيف.

**Returns:**
java.lang.String - اسم العنصر داخل الأرشيف
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


يحصل على الأرشيف الذي ينتمي إليه العنصر.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان العنصر يمثل دليلًا.
### open() {#open--}
```
public final InputStream open()
```


يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل.

الاستخدام:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
