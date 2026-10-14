---
title: "UueArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملفًا مُشفَّرًا بصيغة uu."
type: docs
weight: 128
url: /ar/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

هذه الفئة تمثل ملفًا مُشفَّرًا بصيغة uu.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [UueArchive()](#UueArchive--) | ينشئ مثيلاً جديداً من الفئة [UueArchive](../../com.aspose.zip/uuearchive) المُعدّة للترميز. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | ينشئ مثيلاً جديداً من الفئة [UueArchive](../../com.aspose.zip/uuearchive) المُعدّة للفكّ الترميز. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [UueArchive](../../com.aspose.zip/uuearchive). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج الأرشيف إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج الأرشيف إلى الملف وفق المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكّل أرشيف uue. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getName()](#getName--) | اسم الملف الأصلي. |
| [open()](#open--) | يفتح الأرشيف للفكّ الترميز ويوفر تدفقًا بمحتوى الأرشيف. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المحدد. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | يحفظ الأرشيف إلى ملف الوجهة المحدد. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ترميزه داخل الأرشيف. |
| [setSource(String path)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ترميزه داخل الأرشيف. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


ينشئ مثيلاً جديداً من الفئة [UueArchive](../../com.aspose.zip/uuearchive) المُعدّة للترميز.

المثال التالي يوضح كيفية ترميز ملف باستخدام uuencode.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الترميز. راجع طريقة [open()](../../com.aspose.zip/uuearchive\#open--) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


ينشئ مثيلاً جديداً من الفئة [UueArchive](../../com.aspose.zip/uuearchive).

افتح أرشيفًا من ملف بالمسار وفك ترميزه إلى `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | دفق الوجهة |

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


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكّل أرشيف uue.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - إدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف uue
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


يحصل على الطول.

**Returns:**
java.lang.Long - الطول
### getName() {#getName--}
```
public final String getName()
```


اسم الملف الأصلي.

**Returns:**
java.lang.String - اسم الملف الأصلي
### open() {#open--}
```
public final InputStream open()
```


يفتح الأرشيف للفكّ الترميز ويوفر تدفقًا بمحتوى الأرشيف.

الاستخدام:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outputStream | java.io.OutputStream | دفق الوجهة |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


يحفظ الأرشيف إلى الدفق المقدم.

اكتب البيانات المضغوطة إلى دفق استجابة http.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


يحفظ الأرشيف إلى ملف الوجهة المحدد.

اكتب البيانات المشفرة إلى الملف.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
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


يضبط المحتوى الذي سيتم ترميزه داخل الأرشيف.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
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


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الملف المراد تشفيره |

