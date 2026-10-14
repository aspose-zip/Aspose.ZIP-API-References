---
title: "ArjEntryPlain"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف ARJ."
type: docs
weight: 38
url: /ar/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف ARJ.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | يستخرج مدخل أرشيف ARJ إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على حجم الملف المضغوط. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getName()](#getName--) | يحصل على اسم الإدخال داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


يستخرج مدخل أرشيف ARJ إلى ملف.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف للملف المركّب
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


يحصل على حجم الملف المضغوط.

**Returns:**
long - حجم الملف المضغوط
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


يحصل على اسم الإدخال داخل الأرشيف.

**Returns:**
java.lang.String - اسم المدخل داخل الأرشيف
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


يحصل على حجم الملف الأصلي.

**Returns:**
long - حجم الملف الأصلي
