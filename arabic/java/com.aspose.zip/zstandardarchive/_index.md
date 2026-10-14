---
title: "ZstandardArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف Zstandard."
type: docs
weight: 156
url: /ar/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف Zstandard. استخدمها لإنشاء أرشيفات Zstandard.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive) المُعد للضغط. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive) المُعد للفك. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive) المُعد للفك. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج الأرشيف إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج الأرشيف إلى الملف وفق المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف zstandard. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getName()](#getName--) | يحصل على اسم الإدخال داخل الأرشيف. |
| [open()](#open--) | يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف. |
| [save(File destination)](#save-java.io.File-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String path)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive) المُعد للضغط.

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.zst\");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [open()](../../com.aspose.zip/zstandardarchive\#open--) للفك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive) المُعد للفك.

افتح أرشيفًا من تدفق واستخرجه إلى `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream(\"archive.zst\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [open()](../../com.aspose.zip/zstandardarchive\#open--) للفك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


ينشئ مثيلًا جديدًا من الفئة [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

افتح أرشيفًا من ملف عبر المسار واستخرجه إلى `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة. يجب أن يكون قابلًا للكتابة |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج الأرشيف إلى الملف وفق المسار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله |

**Returns:**
java.io.File - معلومات الملف المستخرج
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج محتوى الأرشيف إلى الدليل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | دليل الوجهة | java.lang.String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

إذا لم يكن الدليل موجودًا، سيتم إنشاؤه |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف zstandard.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف zstandard
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
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
java.lang.String - اسم الإدخال داخل الأرشيف
### open() {#open--}
```
public final InputStream open()
```


يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف.

يستخرج الأرشيف وينسخ المحتوى المستخرج إلى تدفق الملف.

```

``````

try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
try (FileOutputStream extracted = new FileOutputStream(\"data.bin\")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.File | الملف الذي سيُفتح ك تدفق وجهة |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File(\"archive.zst\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outputStream | java.io.OutputStream | دفق الوجهة |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


يحفظ الأرشيف إلى الدفق المقدم.

اكتب البيانات المضغوطة إلى دفق استجابة http.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| file | java.io.File | المرجع إلى ملف ليتم ضغطه |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.zst\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الملف ليتم ضغطه |

