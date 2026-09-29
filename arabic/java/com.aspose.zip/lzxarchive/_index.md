---
title: "LzxArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف LZX .lzx."
type: docs
weight: 89
url: /ar/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف LZX (.lzx).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات والمجلدات في الأرشيف إلى الدليل المحدد. |
| [getEntries()](#getEntries--) | يحصل على إدخالات الملفات من نوع [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | java.io.InputStream | مصدر الأرشيف. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | java.io.InputStream | مصدر الأرشيف. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


يُنشئ كائنًا جديدًا من الفئة [LzxArchive](../../com.aspose.zip/lzxarchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يستخرج أرشيفًا، ثم يفك ضغط الإدخال الأول إلى `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار المؤهل بالكامل أو المسار النسبي لملف الأرشيف. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات والمجلدات في الأرشيف إلى الدليل المحدد.

```

``````

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
