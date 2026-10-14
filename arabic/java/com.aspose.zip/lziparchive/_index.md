---
title: "LzipArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف Lzip."
type: docs
weight: 83
url: /ar/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف Lzip. استخدمها لإنشاء أو استخراج أرشيفات Lzip.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | يُنشئ مثيلًا جديدًا من [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | يُنشئ مثيلًا جديدًا من [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | يستخرج أرشيف lzip إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج أرشيف lzip إلى تدفق. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج أرشيف lzip إلى ملف حسب المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على المدخلات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف lzip. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على الطول. |
| [getName()](#getName--) | اسم الملف الأصلي. |
| [getSettings()](#getSettings--) | يحصل على إعداد أرشيف lzip المحدد. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم البيانات غير المضغوطة للملف بالبايت. |
| [save(File destination)](#save-java.io.File-) | يحفظ أرشيف lzip إلى ملف الوجهة المقدم. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | يحفظ أرشيف lzip إلى التدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ أرشيف lzip إلى ملف الوجهة المقدم. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String path)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


يُنشئ مثيلًا جديدًا من [LzipArchive](../../com.aspose.zip/lziparchive).

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


يُنشئ مثيلًا جديدًا من [LzipArchive](../../com.aspose.zip/lziparchive).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | إعداد أرشيف lzip المحدد مع تعريف حجم القاموس |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | خيارات لتحميل الأرشيف. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


يُنشئ مثيلًا جديدًا من الفئة [LzipArchive](../../com.aspose.zip/lziparchive) المُعد لفك الضغط.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى مصدر الأرشيف |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | خيارات لتحميل الأرشيف. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


يستخرج أرشيف lzip إلى ملف.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
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


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
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


يستخرج أرشيف lzip إلى ملف حسب المسار.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
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
java.io.File - the file info of the extracted file
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


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.File | الملف، الذي سيفتح كدفق وجهة |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


يحفظ أرشيف lzip إلى التدفق المقدم.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
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

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | دفق الإدخال للأرشيف |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

