---
title: "GzipArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف gzip."
type: docs
weight: 69
url: /ar/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

تمثل هذه الفئة ملف أرشيف gzip. استخدمها لإنشاء أو استخراج أرشيفات gzip.

خوارزمية ضغط Gzip تستند إلى خوارزمية DEFLATE، التي هي مزيج من LZ77 وترميز هوفمان.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد للضغط. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج الأرشيف إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج الأرشيف إلى الملف وفق المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على مدخلات من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف gzip. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على حجم الملف الأصلي. |
| [getName()](#getName--) | اسم الملف الأصلي. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم الملف الأصلي. |
| [open()](#open--) | يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String path)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد للضغط.

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. انظر طريقة [open()](../../com.aspose.zip/gziparchive\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط.

افتح أرشيفًا من تدفق واستخرجه إلى `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. انظر طريقة [open()](../../com.aspose.zip/gziparchive\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | خيارات لتحميل الأرشيف. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive) المُعد لفك الضغط.

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. انظر طريقة [open()](../../com.aspose.zip/gziparchive\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الأرشيف. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


ينشئ مثيلاً جديدًا من الفئة [GzipArchive](../../com.aspose.zip/gziparchive).

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | تدفق الوجهة. يجب أن يكون قابلًا للكتابة. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج الأرشيف إلى الملف وفق المسار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |

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

إذا لم يكن الدليل موجودًا، فسيتم إنشاؤه. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على مدخلات من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف gzip.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - مدخلات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف gzip.
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


يحصل على حجم الملف الأصلي.

أثناء فك الضغط، قد تحتوي هذه الخاصية على حجم غير صحيح. إذا تجاوز حجم الملف غير المضغوط 4 جيجابايت، ستعطي هذه الخاصية قيمة خاطئة بسبب حد 32 بت في الرأس.

**Returns:**
java.lang.Long - حجم ملف أصلي
### getName() {#getName--}
```
public final String getName()
```


اسم الملف الأصلي.

**Returns:**
java.lang.String - اسم الملف الأصلي
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


يحصل على حجم الملف الأصلي.

أثناء فك الضغط، قد تحتوي هذه الخاصية على حجم غير صحيح. إذا تجاوز حجم الملف غير المضغوط 4 جيجابايت، ستعطي هذه الخاصية قيمة خاطئة بسبب حد 32 بت في الرأس.

**Returns:**
long - حجم ملف أصلي.
### open() {#open--}
```
public final InputStream open()
```


يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف.

يستخرج الأرشيف وينسخ المحتوى المستخرج إلى تدفق الملف.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | دفق الوجهة. |

`outputStream` يجب أن يكون قابلًا للكتابة. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

استخدم هذه الطريقة لتكوين أرشيف tar.gz مشترك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | أرشيف Tar ليتم ضغطه. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | دفق الإدخال للأرشيف. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

