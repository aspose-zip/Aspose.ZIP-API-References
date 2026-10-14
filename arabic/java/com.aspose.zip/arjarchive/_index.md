---
title: "ArjArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف ARJ."
type: docs
weight: 37
url: /ar/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف ARJ.

الطرق التالية للضغط فقط مدعومة:

| ------ | ------------------------------------------------------------ |
| الطريقة | الشرح                                                  |
| 0      | غير مضغوط                                                 |
| 1      | مزيج من LZ77 وترميز هوفمان التكيفي. أفضل نسبة. |
| 2      | مزيج من LZ77 وترميز هوفمان التكيفي.             |
| 3      | مزيج من LZ77 وترميز هوفمان التكيفي. أفضل سرعة. |
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الإدخالات إلى الدليل المحدد. |
| [getCommentary()](#getCommentary--) | يحصل على التعليق. |
| [getEntries()](#getEntries--) | يحصل على الإدخالات من نوع [ArjEntryPlain](../../com.aspose.zip/arjentryplain) التي تشكل أرشيف ARJ. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getName()](#getName--) | يحصل على الاسم الأصلي. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | java.io.InputStream | مصدر الأرشيف |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | java.io.InputStream | مصدر الأرشيف |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


يُنشئ مثيلًا جديدًا من الفئة [ArjArchive](../../com.aspose.zip/arjarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يفتح ضغط أي إدخال. راجع طريقة [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الإدخالات إلى الدليل المحدد.

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى دليل:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
