---
title: "WimArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف wim."
type: docs
weight: 130
url: /ar/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف wim.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج الأرشيف إلى الملف وفق المسار. |
| [getBootImageIndex()](#getBootImageIndex--) | يحصل على الفهرس (المبني على الصفر) لصورة الإقلاع. |
| [getEntries()](#getEntries--) | يحصل على إدخالات من نوع [WimEntry](../../com.aspose.zip/wimentry) تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على إدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) تشكل أرشيف wim. |
| [getFileFormatVersion()](#getFileFormatVersion--) | يحصل على نسخة تنسيق الملف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getGuid()](#getGuid--) | يحصل على UUID التعريفي للأرشيف. |
| [getImages()](#getImages--) | يحصل على إدخالات من نوع [WimImage](../../com.aspose.zip/wimimage) تشكل الأرشيف. |
| [getManifest()](#getManifest--) | يحصل على البيان المدمج الذي يصف الملف والصور المحتواة. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى دليل.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

هذا المنشئ لا يفك أي إدخال. راجع طريقة [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


يُنشئ مثيلًا جديدًا من الفئة [WimArchive](../../com.aspose.zip/wimarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى دليل.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

هذا المنشئ لا يفك أي إدخال. راجع طريقة [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) لفك الضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | خيارات لتحميل الأرشيف الموجود. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج الأرشيف إلى الملف وفق المسار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | مسار الدليل الذي توضع فيه الملفات المستخرجة |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


يحصل على الفهرس (المبني على الصفر) لصورة الإقلاع.

**Returns:**
int - الفهرس (المبني على الصفر) لصورة الإقلاع
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


يحصل على إدخالات من نوع [WimEntry](../../com.aspose.zip/wimentry) تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - الإدخالات التي تشكل الأرشيف
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على إدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) تشكل أرشيف wim.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف wim
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


يحصل على نسخة تنسيق الملف.

**Returns:**
int - إصدار تنسيق الملف
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


يحصل على UUID التعريفي للأرشيف.

**Returns:**
java.util.UUID - معرف UUID للأرشيف
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


يحصل على إدخالات من نوع [WimImage](../../com.aspose.zip/wimimage) تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - الإدخالات من نوع [WimImage](../../com.aspose.zip/wimimage) التي تشكل الأرشيف
### getManifest() {#getManifest--}
```
public final String getManifest()
```


يحصل على البيان المدمج الذي يصف الملف والصور المحتواة.

**Returns:**
java.lang.String - البيان المدمج الذي يصف الملف والصور المحتواة
