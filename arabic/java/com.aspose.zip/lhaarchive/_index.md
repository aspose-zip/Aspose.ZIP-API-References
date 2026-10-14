---
title: "LhaArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف LHA .lzh."
type: docs
weight: 75
url: /ar/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف LHA (.lzh).

الطرق التالية للضغط فقط مدعومة:

| ------ | --------------------------------------------- |
| الطريقة | الشرح                                   |
| lh0    | غير مضغوط                                  |
| lh4    | قاموس انزلاقي 8 KiB وشفرة هوفمان ثابتة   |
| lh5    | قاموس انزلاقي 16 KiB وشفرة هوفمان ثابتة  |
| lh6    | قاموس انزلاقي 64 KiB وشفرة هوفمان ثابتة  |
| lh7    | قاموس منزلق بحجم 128 KiB و Huffman ثابت |
| lhx    | قاموس منزلق بحجم 1 Mib و Huffman ثابت   |
| lhd    | دليل                                     |
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات والمجلدات في الأرشيف إلى الدليل المحدد. |
| [getEntries()](#getEntries--) | يحصل على إدخالات الملفات من النوع [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


يُنشئ مثلاً جديداً من الفئة [LhaArchive](../../com.aspose.zip/lhaarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يستخرج أرشيفًا، ثم يفك ضغط الإدخال الأول إلى `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار المؤهل بالكامل أو المسار النسبي لملف الأرشيف. |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | خيارات لتحميل الأرشيف الموجود. |

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

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
