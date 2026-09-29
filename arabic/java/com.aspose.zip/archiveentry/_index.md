---
title: "ArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل ملفًا واحدًا داخل الأرشيف."
type: docs
weight: 27
url: /ar/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

يمثل ملفًا واحدًا داخل الأرشيف.

تحويل كائن [ArchiveEntry](../../com.aspose.zip/archiveentry) إلى [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) لتحديد ما إذا كان الإدخال مشفرًا أم لا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getComment()](#getComment--) | يحصل على تعليق الإدخال داخل الأرشيف. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على حجم الملف المضغوط. |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على الإعدادات للضغط أو فك الضغط. |
| [getDataSource()](#getDataSource--) | المصدر للإدخال إذا تم إضافة الإدخال إلى الأرشيف، وليس استخراجًا. |
| [getExtractionProgressed()](#getExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getModificationTime()](#getModificationTime--) | يحصل على تاريخ ووقت التعديل الأخير. |
| [getName()](#getName--) | يحصل على اسم الإدخال داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |
| [open(String password)](#open-java.lang.String-) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | يضبط تاريخ ووقت التعديل الأخير. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخراج إدخال من أرشيف zip باستخدام كلمة مرور.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | تدفق الوجهة. يجب أن يكون قابلًا للكتابة. |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لفك التشفير. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج المدخل إلى نظام الملفات بالمسار المقدم.

استخراج إدخالين من أرشيف ZIP، كل منهما بكلمة مرور خاصة.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لفك التشفير. |

**Returns:**
java.io.File - معلومات الملف المستخرج
### getComment() {#getComment--}
```
public final String getComment()
```


يحصل على تعليق الإدخال داخل الأرشيف.

**Returns:**
java.lang.String - تعليق على العنصر داخل الأرشيف
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


يحصل على حجم الملف المضغوط.

**Returns:**
long - حجم الملف المضغوط
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

في هذا المثال يتم استخدام معالج الحدث للإلغاء بعد استخراج أول مئة ميغابايت من العنصر.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

اقرأ من الدفق للحصول على المحتوى الأصلي للملف.

**Returns:**
java.io.InputStream - الدفق الذي يمثل محتويات العنصر.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط.


الاستخدام:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

مرسل الحدث هو كائن من نوع [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | حدث يتم إطلاقه عندما يتم ضغط جزء من الدفق الخام. |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


يضبط حدثًا يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام.

في هذا المثال يتم استخدام معالج الحدث لحساب نسبة الحجم المعالج بالنسب المئوية.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

المرسل Event هو كائن من نوع [ArchiveEntry](../../com.aspose.zip/archiveentry). يمكن إلغاء الاستخراج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | حدث يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


يضبط تاريخ ووقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.util.Date | تاريخ ووقت آخر تعديل |

