---
title: "TarEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف tar."
type: docs
weight: 126
url: /ar/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف tar.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getModificationTime()](#getModificationTime--) | يحصل على وقت التعديل للملف أو الدليل. |
| [getName()](#getName--) | يحصل على اسم العنصر داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم العنصر داخل الأرشيف. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخراج عنصر من أرشيف tar.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف المستخرج
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


يحصل على وقت التعديل للملف أو الدليل.

**Returns:**
java.util.Date - وقت تعديل الملف أو الدليل.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم العنصر داخل الأرشيف.

**Returns:**
java.lang.String - اسم العنصر داخل الأرشيف
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


يحصل على حجم الملف الأصلي.

لها نفس القيمة مثل `Length`([getLength](../../com.aspose.zip/tarentry\\#getLength--))

**Returns:**
long - حجم الملف الأصلي.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا
### open() {#open--}
```
public final InputStream open()
```


يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل.


الاستخدام:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

