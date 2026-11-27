---
title: "XzArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف xz."
type: docs
weight: 146
url: /ar/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف xz. استخدمها لإنشاء واستخراج أرشيفات xz.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XzArchive()](#XzArchive--) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) ويُكوّن الأرشيف بتنسيق xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) ويُكوّن الأرشيف بتنسيق xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | يستخرج أرشيف xz إلى ملف. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | يستخرج أرشيف xz إلى تدفق. |
| [extract(String path)](#extract-java.lang.String-) | يستخرج أرشيف xz إلى ملف عبر المسار. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج محتوى الأرشيف إلى الدليل المحدد. |
| [getFileEntries()](#getFileEntries--) | يحصل على المدخلات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكّل أرشيف xz. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getLength()](#getLength--) | يحصل على طول المدخل بالبايت. |
| [getName()](#getName--) | يحصل على اسم الإدخال داخل الأرشيف. |
| [getUncompressedSize()](#getUncompressedSize--) | يحصل على حجم البيانات غير المضغوطة للملف بالبايت. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ أرشيف xz إلى التدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ أرشيف xz إلى ملف الوجهة المقدم. |
| [setSource(File file)](#setSource-java.io.File-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) ويُكوّن الأرشيف بتنسيق xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) ويُكوّن الأرشيف بتنسيق xz.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | مجموعة من إعدادات أرشيف xz الخاصة: حجم القاموس، حجم الكتلة، نوع الفحص |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط.

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط.

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | خيارات لتحميل الأرشيف. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط.

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى مصدر الأرشيف |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


ينشئ مثيلاً جديدًا للفئة [XzArchive](../../com.aspose.zip/xzarchive) مُجهّزًا لفك الضغط.

هذا المُنشئ لا يقوم بفك الضغط. راجع طريقة [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى مصدر الأرشيف |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


يستخرج أرشيف xz إلى ملف.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | java.io.OutputStream | تدفق لتخزين البيانات غير المضغوطة |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


يستخرج أرشيف xz إلى ملف عبر المسار.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

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

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


يحفظ أرشيف xz إلى ملف الوجهة المقدم.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| file | java.io.File | ملف سيتم فتحه كتيار إدخال |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourcePath | java.lang.String | المسار إلى الملف الذي سيتم فتحه كتيار إدخال |

