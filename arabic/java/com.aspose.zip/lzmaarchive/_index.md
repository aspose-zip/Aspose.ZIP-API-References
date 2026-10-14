---
title: "LzmaArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف LZMA."
type: docs
weight: 86
url: /ar/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

تمثل هذه الفئة ملف أرشيف LZMA. استخدمها لإنشاء أو استخراج أرشيفات LZMA.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) ويُكوِّن الأرشيف بصيغة lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) ويُكوِّن الأرشيف بصيغة lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) مُعدًا لفك الضغط. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) مُعدًا لفك الضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | يستخرج أرشيف lzma إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج أرشيف lzma إلى تدفق. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج أرشيف lzma إلى ملف حسب المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على إدخالات من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف lzma. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getName()](#getName--) | اسم الملف الأصلي. |
| [save(File destination)](#save-java.io.File-) | يحفظ أرشيف lzma إلى ملف الوجهة المحدد. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ أرشيف lzma إلى التدفق المحدد. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ أرشيف lzma إلى ملف الوجهة المحدد. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) ويُكوِّن الأرشيف بصيغة lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) ويُكوِّن الأرشيف بصيغة lzma.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | مجموعة من إعدادات أرشيف lzma المحدد. |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) مُعدًا لفك الضغط.

هذا المُنشئ لا يفك الضغط. راجع طريقة [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


يُنشئ مثيلًا جديدًا من الفئة [LzmaArchive](../../com.aspose.zip/lzmaarchive) مُعدًا لفك الضغط.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| file | java.io.File | الملف لتخزين البيانات غير المضغوطة |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


يستخرج أرشيف lzma إلى تدفق.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى الملف الذي سيخزن البيانات غير المضغوطة |

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


يحصل على إدخالات من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - إدخالات من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف lzma.
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
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


يحفظ أرشيف lzma إلى ملف الوجهة المحدد.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ أرشيف lzma إلى ملف الوجهة المحدد.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| file | java.io.File | الملف الذي سيتم فتحه كدفق إدخال |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourcePath | java.lang.String | مسار الملف الذي سيتم فتحه كدفق إدخال |

