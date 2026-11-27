---
title: "AppleArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل ملفًا أو دليلًا داخل ."
type: docs
weight: 17
url: /ar/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

يمثل ملفًا أو دليلًا داخل [AppleArchive](../../com.aspose.zip/applearchive).

يمكن لنسخة من هذه الفئة أن تمثل إما إدخالًا تم تحليله من أرشيف Apple موجود أو إدخالًا تمت إضافته إلى أرشيف يتم تكوينه.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج إدخال أرشيف Apple إلى نظام ملفات حسب المسار. |
| [getLength()](#getLength--) | يحصل على الطول غير المضغوط للإدخال بالبايت. |
| [getName()](#getName--) | يحصل على مسار الإدخال داخل الأرشيف. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة. يجب أن يكون قابلًا للكتابة |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج إدخال أرشيف Apple إلى نظام ملفات حسب المسار.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
