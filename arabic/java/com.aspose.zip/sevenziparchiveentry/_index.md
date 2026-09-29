---
title: "SevenZipArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل ملفًا واحدًا داخل أرشيف 7z."
type: docs
weight: 105
url: /ar/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

تمثل ملفًا واحدًا داخل أرشيف 7z.

حوّل كائن [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) إلى [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) لتحديد ما إذا كان العنصر مشفرًا أم لا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | يستخرج المدخل إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | يستخرج المدخل إلى نظام الملفات بالمسار المقدم. |
| [getCompressedSize()](#getCompressedSize--) | يحصل على حجم الملف المضغوط. |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على الإعدادات للضغط أو فك الضغط. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getModificationTime()](#getModificationTime--) | يحصل على تاريخ ووقت التعديل الأخير. |
| [getName()](#getName--) | يحصل على اسم العنصر داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [isDirectory()](#isDirectory--) | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [open()](#open--) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
| [open(String password)](#open-java.lang.String-) | يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج المدخل إلى الدفق المقدم.

استخراج إدخال من أرشيف zip باستخدام كلمة مرور.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة. يجب أن يكون قابلًا للكتابة |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لفك التشفير |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج المدخل إلى نظام الملفات بالمسار المقدم.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.getEntries().get(0).extract("data.bin");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |
| كلمة المرور | java.lang.String | كلمة مرور اختيارية لفك التشفير |

**Returns:**
java.io.File - معلومات الملف المستخرج
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

**Returns:**
java.io.InputStream - الدفق الذي يمثل محتويات العنصر
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


يفتح المدخل للاستخراج ويوفر دفقًا بمحتوى المدخل.

الاستخدام:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

مرسل الحدث هو كائن [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

لا يتم الاستدعاء في وضع الصلب وفي الوضع متعدد الخيوط لإدخالات LZMA2.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | حدث يتم إطلاقه عندما يتم ضغط جزء من الدفق الخام. |

