---
title: "Lz4Archive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف LZ4."
type: docs
weight: 80
url: /ar/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف LZ4. استخدمها لاستخراج أو إنشاء أرشيفات LZ4.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد لفك الضغط. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد لفك الضغط. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive()](#Lz4Archive--) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد للضغط. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد للضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج الأرشيف إلى الدفق المقدم. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج الأرشيف إلى الملف وفق المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getName()](#getName--) | يحصل على الاسم الأصلي. |
| [open()](#open--) | يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف. |
| [save(File destination)](#save-java.io.File-) | يحفظ أرشيف lz4 إلى ملف الوجهة المقدم. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ أرشيف lz4 إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String path)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد لفك الضغط.

افتح أرشيفاً من دفق واستخرجها إلى `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [open()](../../com.aspose.zip/lz4archive\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | الخيارات لتحميل الأرشيف بها. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive).

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [open()](../../com.aspose.zip/lz4archive\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | الخيارات لتحميل الأرشيف بها. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد للضغط.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


يُنشئ مثيلاً جديداً من الفئة [Lz4Archive](../../com.aspose.zip/lz4archive) المُعد للضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | إعدادات الأرشيف المُركب. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج الأرشيف إلى الدفق المقدم.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

**Returns:**
java.io.InputStream - الدفق الذي يمثل محتويات الأرشيف
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


يحفظ أرشيف lz4 إلى ملف الوجهة المقدم.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lz4"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(\"data.bin\");
archive.save("archive.lz4");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

استخدم هذه الطريقة لإنشاء أرشيف tar.lz4 مشترك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | أرشيف Tar ليتم ضغطه. |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileInfo | java.io.File | المرجع إلى ملف ليتم ضغطه. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.lz4");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى الملف ليتم ضغطه. |

