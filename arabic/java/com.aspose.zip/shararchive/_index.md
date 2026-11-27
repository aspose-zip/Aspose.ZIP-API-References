---
title: "SharArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف shar."
type: docs
weight: 119
url: /ar/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

هذه الفئة تمثل ملف أرشيف shar.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SharArchive()](#SharArchive--) | يُنشئ مثيلاً جديدًا من الفئة [SharArchive](../../com.aspose.zip/shararchive). |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | يُنشئ مثيلاً جديدًا من الفئة [SharArchive](../../com.aspose.zip/shararchive) مُعدًا لفك الضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | إنشاء إدخال واحد داخل الأرشيف. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | إنشاء إدخال واحد داخل الأرشيف. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | يزيل الظهور الأول لإدخال محدد من قائمة الإدخالات. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | يزيل الإدخال من قائمة الإدخالات حسب الفهرس. |
| [getEntries()](#getEntries--) | يحصل على الإدخالات من نوع [SharEntry](../../com.aspose.zip/sharentry) التي تُشكل الأرشيف. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


يُنشئ مثيلاً جديدًا من الفئة [SharArchive](../../com.aspose.zip/shararchive).

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | java.io.File | المجلد المراد ضغطه |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | java.lang.String | المجلد المراد ضغطه |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| file | java.io.File | البيانات الوصفية للملف أو المجلد المراد ضغطه |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| source | java.io.InputStream | دفق الإدخال للعنصر |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


إنشاء إدخال واحد داخل الأرشيف.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

يتم تعيين اسم المدخل فقط داخل معامل `name`. اسم الملف المقدم في معامل `sourcePath` لا يؤثر على اسم المدخل.

إذا تم فتح الملف فورًا باستخدام معامل `openImmediately` يصبح محجوزًا حتى يتم التخلص من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| sourcePath | java.lang.String | المسار إلى الملف المراد ضغطه |
| openImmediately | boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


يزيل الظهور الأول لإدخال محدد من قائمة الإدخالات.

إليك كيفية إزالة جميع العناصر باستثناء الأخير:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| entryIndex | int | المؤشر الصفري للعنصر المراد إزالته |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


يحصل على الإدخالات من نوع [SharEntry](../../com.aspose.zip/sharentry) التي تُشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - الإدخالات من نوع [SharEntry](../../com.aspose.zip/sharentry) التي تُشكل الأرشيف
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


يحفظ الأرشيف إلى الدفق المقدم.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(sharFile);
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


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

من الممكن حفظ الأرشيف إلى نفس المسار الذي تم تحميله منه. ومع ذلك، لا يُنصح بذلك لأن هذا الأسلوب يستخدم النسخ إلى ملف مؤقت |

