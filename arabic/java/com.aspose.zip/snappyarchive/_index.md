---
title: "SnappyArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف snappy."
type: docs
weight: 121
url: /ar/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف snappy. استخدمها لإنشاء أو استخراج أرشيفات snappy.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | ينشئ مثيلًا جديدًا من الفئة [SnappyArchive](../../com.aspose.zip/snappyarchive) مُعد للضغط. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | ينشئ مثيلًا جديدًا من الفئة [SnappyArchive](../../com.aspose.zip/snappyarchive) مُعد للفك. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | ينشئ مثيلًا جديدًا من الفئة [SnappyArchive](../../com.aspose.zip/snappyarchive) مُعد للفك. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | يستخرج أرشيف Snappy إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج أرشيف Snappy إلى تدفق. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج أرشيف Snappy إلى ملف عبر المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على إدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف Snappy. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getName()](#getName--) | اسم الملف الأصلي. |
| [save(File destination)](#save-java.io.File-) | يحفظ أرشيف Snappy إلى ملف الوجهة المُقدم. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ أرشيف Snappy إلى التدفق المُقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ أرشيف Snappy إلى ملف الوجهة المُقدم. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


ينشئ مثيلًا جديدًا من الفئة [SnappyArchive](../../com.aspose.zip/snappyarchive) مُعد للضغط.

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) للفك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى مصدر الأرشيف |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


يستخرج أرشيف Snappy إلى ملف.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | التدفق لتخزين البيانات المفكوكة |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج أرشيف Snappy إلى ملف عبر المسار.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.File | الملف الذي سيتم فتحه كتدفق وجهة |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


يحفظ أرشيف Snappy إلى التدفق المُقدم.

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(\"data.bin\");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | دفق الإدخال للأرشيف |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

