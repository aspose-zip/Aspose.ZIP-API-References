---
title: "LzxArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف LZX."
type: docs
weight: 90
url: /ar/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف LZX.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج مدخل أرشيف Lzx إلى نظام ملفات حسب المسار. |
| [getCommentary()](#getCommentary--) | يحصل على التعليق. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على حجم الملف المضغوط. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getModificationTime()](#getModificationTime--) | يحصل على وقت التعديل الأخير للإدخال. |
| [getName()](#getName--) | يحصل على اسم الإدخال. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان هذا الإدخال مجلدًا. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | تدفق الوجهة. يجب أن يكون قابلًا للكتابة. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج مدخل أرشيف Lzx إلى نظام ملفات حسب المسار.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
