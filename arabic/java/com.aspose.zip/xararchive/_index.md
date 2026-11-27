---
title: "XarArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف xar."
type: docs
weight: 136
url: /ar/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف xar.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XarArchive()](#XarArchive--) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | إنشاء إدخال واحد داخل الأرشيف. |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | يزيل الظهور الأول لإدخال محدد من قائمة الإدخالات. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد. |
| [getEntries()](#getEntries--) | يحصل على الإدخالات من نوع [XarEntry](../../com.aspose.zip/xarentry) التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف xar. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive).

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | إعدادات الضغط الافتراضية، المطبقة على جميع إدخالات الأرشيف |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

هذا المُنشئ لا يفك أي مدخل. راجع طريقة [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | الخيارات لتحميل الأرشيف |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


ينشئ مثيلاً جديداً من الفئة [XarArchive](../../com.aspose.zip/xararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

هذا المُنشئ لا يفك أي مدخل. راجع طريقة [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | الخيارات لتحميل الأرشيف |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | java.io.File | الدليل للضغط |
| includeRootDirectory | boolean | يشير إلى ما إذا كان يجب تضمين الدليل الجذر نفسه أم لا |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | java.lang.String | الدليل للضغط |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | java.lang.String | الدليل للضغط |
| includeRootDirectory | boolean | يشير إلى ما إذا كان يجب تضمين الدليل الجذر نفسه أم لا |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | إعدادات الضغط المستخدمة للعناصر المضافة من نوع [XarEntry](../../com.aspose.zip/xarentry) |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

إذا تم فتح الملف فورًا باستخدام معامل `openImmediately` يصبح محجوزًا حتى يتم التخلص من الأرشيف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| file | java.io.File | البيانات الوصفية للملف أو المجلد المراد ضغطه |
| openImmediately | boolean | صحيح إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| source | java.io.InputStream | دفق الإدخال للعنصر |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

يتم تعيين اسم المدخل فقط داخل معامل `name`. اسم الملف المقدم في معامل `sourcePath` لا يؤثر على اسم المدخل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| sourcePath | java.lang.String | المسار إلى الملف الذي سيتم ضغطه |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

يتم تعيين اسم المدخل فقط داخل معامل `name`. اسم الملف المقدم في معامل `sourcePath` لا يؤثر على اسم المدخل.

إذا تم فتح الملف فورًا باستخدام معامل `openImmediately` يصبح محجوزًا حتى يتم التخلص من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| sourcePath | java.lang.String | المسار إلى الملف الذي سيتم ضغطه |
| openImmediately | boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | إعدادات الضغط المستخدمة للعنصر المضاف من نوع [XarEntry](../../com.aspose.zip/xarentry) |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


يزيل الظهور الأول لإدخال محدد من قائمة الإدخالات.

إليك كيفية إزالة جميع العناصر باستثناء الأخير:

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | دليل الوجهة | java.lang.String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

إذا لم يكن الدليل موجودًا، سيتم إنشاؤه |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


يحصل على الإدخالات من نوع [XarEntry](../../com.aspose.zip/xarentry) التي تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - عناصر من نوع [XarEntry](../../com.aspose.zip/xarentry) تشكل الأرشيف
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف xar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - عناصر من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) تشكل أرشيف xar
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


يحفظ الأرشيف إلى الدفق المقدم.

لأرشيفات كبيرة استخدم [save(String)](../../com.aspose.zip/xararchive\#save-String-) بدلاً من الحفظ إلى java.io.FileOutputStream.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


يحفظ الأرشيف إلى الدفق المقدم.

لأرشيفات كبيرة استخدم [save(String)](../../com.aspose.zip/xararchive\#save-String-) بدلاً من الحفظ إلى java.io.FileOutputStream.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | الخيارات لحفظ أرشيف xar باستخدام |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | الخيارات لحفظ أرشيف xar باستخدام |

