---
title: "RarArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل ملفًا واحدًا داخل الأرشيف."
type: docs
weight: 98
url: /ar/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

يمثل ملفًا واحدًا داخل الأرشيف.

حوّل كائن [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) إلى [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) لتحديد ما إذا كان الإدخال مشفرًا أم لا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على حجم الملف المضغوط. |
| [getCreationTime()](#getCreationTime--) | يحصل على تاريخ ووقت الإنشاء. |
| [getExtractionProgressed()](#getExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |
| [getLastAccessTime()](#getLastAccessTime--) | يحصل على تاريخ ووقت آخر وصول. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getModificationTime()](#getModificationTime--) | يحصل على تاريخ ووقت التعديل الأخير. |
| [getName()](#getName--) | يحصل على اسم العنصر داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |
| [open(String password)](#open-java.lang.String-) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.


استخراج إدخال من أرشيف rar باستخدام كلمة مرور.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
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


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
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


استخراج إدخالين من أرشيف rar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
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
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


يحصل على حجم الملف المضغوط.

**Returns:**
long - حجم الملف المضغوط
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


يحصل على تاريخ ووقت الإنشاء.

**Returns:**
java.util.Date - تاريخ ووقت الإنشاء.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


يحصل على حدث يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
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

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

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
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

مرسل الحدث هو كائن [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | حدث يتم إطلاقه عندما يتم استخراج جزء من تدفق البيانات الخام. |

