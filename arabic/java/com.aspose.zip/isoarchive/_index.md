---
title: "IsoArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل أرشيف ISO ISO 9660."
type: docs
weight: 71
url: /ar/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

تمثل أرشيف ISO (ISO 9660).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُنشئ أرشيف ISO فارغ لإضافة ملفات ودلائل جديدة. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | يضيف دليلًا إلى صورة ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | يضيف ملفًا إلى صورة ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | يضيف ملفًا إلى صورة ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | يضيف ملفًا إلى صورة ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الإدخالات إلى الدليل المحدد. |
| [getEntries()](#getEntries--) | يحصل على الإدخالات من نوع [IsoEntry](../../com.aspose.zip/isoentry) التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | يحفظ صورة ISO إلى الدفق المحدد. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | يحفظ صورة ISO إلى الدفق المحدد. |
| [save(String path)](#save-java.lang.String-) | يحفظ صورة ISO إلى المسار المحدد. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | يحفظ صورة ISO إلى المسار المحدد. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُنشئ أرشيف ISO فارغ لإضافة ملفات ودلائل جديدة.

المثال التالي يوضح كيفية إنشاء أرشيف ISO فارغ جديد وإضافة ملفات إليه:

```

``````

// إنشاء أرشيف ISO فارغ جديد
try (IsoArchive isoArchive = new IsoArchive()) {
// إضافة ملفات إلى أرشيف ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// حفظ أرشيف ISO إلى ملف
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يفك أي عنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

هذا المُنشئ لا يفك أي عنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


ينشئ نسخة جديدة من الفئة [IsoArchive](../../com.aspose.zip/isoarchive) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | الدليل لاستخراج العناصر إليه |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


يحصل على الإدخالات من نوع [IsoEntry](../../com.aspose.zip/isoentry) التي تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - عناصر من نوع [IsoEntry](../../com.aspose.zip/isoentry) التي تشكل أرشيف iso
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - عناصر من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف iso
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


يحفظ صورة ISO إلى الدفق المحدد.

المثال التالي يوضح كيفية حفظ أرشيف ISO إلى تدفق الذاكرة:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// إنشاء أرشيف ISO فارغ جديد
try (IsoArchive isoArchive = new IsoArchive()) {
// إضافة ملفات إلى أرشيف ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// حفظ أرشيف ISO إلى تدفق الذاكرة
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.OutputStream | دفق البيانات حيث سيتم حفظ صورة ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | الخيارات لحفظ أرشيف ISO باستخدام |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


يحفظ صورة ISO إلى المسار المحدد.

المثال التالي يوضح كيفية حفظ أرشيف ISO إلى ملف:

```

``````

// إنشاء أرشيف ISO فارغ جديد
try (IsoArchive isoArchive = new IsoArchive()) {
// إضافة ملفات إلى أرشيف ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// حفظ أرشيف ISO إلى ملف
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار حيث سيتم حفظ صورة ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | الخيارات لحفظ أرشيف ISO باستخدام |

