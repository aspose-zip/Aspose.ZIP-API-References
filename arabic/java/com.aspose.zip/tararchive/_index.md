---
title: "TarArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف أرشيف tar."
type: docs
weight: 125
url: /ar/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف أرشيف tar. استخدمها لإنشاء أو استخراج أو تحديث أرشيفات tar.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [TarArchive()](#TarArchive--) | ينشئ مثيلًا جديدًا من الفئة [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | ينشئ مثيلاً جديداً من الفئة [Archive](../../com.aspose.zip/archive) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | ينشئ مثيلًا جديدًا من الفئة [TarArchive](../../com.aspose.zip/tararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | يزيل الظهور الأول لإدخال محدد من قائمة الإدخالات. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | يزيل الإدخال من قائمة الإدخالات حسب الفهرس. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | يستخرج أرشيف gzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | يستخرج أرشيف gzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | يستخرج أرشيف LZ4 المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | يستخرج أرشيف LZ4 المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | يستخرج أرشيف LZMA المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | يستخرج أرشيف LZMA المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | يستخرج أرشيف lzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | يستخرج أرشيف lzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | يستخرج أرشيف بصيغة xz المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromXz(String path)](#fromXz-java.lang.String-) | يستخرج أرشيف بصيغة xz المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | يستخرج أرشيف بصيغة Z المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromZ(String path)](#fromZ-java.lang.String-) | يستخرج أرشيف بصيغة Z المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | يستخرج أرشيف Zstandard المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | يستخرج أرشيف Zstandard المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة. |
| [getEntries()](#getEntries--) | يحصل على إدخالات من نوع [TarEntry](../../com.aspose.zip/tarentry) التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف tar. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق مع ضغط gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق مع ضغط gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق باستخدام ضغط LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق باستخدام ضغط LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق باستخدام ضغط LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق باستخدام ضغط LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق مع ضغط lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق مع ضغط lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق مع ضغط xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق مع ضغط xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | يحفظ الأرشيف إلى الدفق مع ضغط xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق مع ضغط Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق مع ضغط Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق مع ضغط Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الدفق مع ضغط Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


ينشئ مثيلًا جديدًا من الفئة [TarArchive](../../com.aspose.zip/tararchive).

المثال التالي يوضح كيفية ضغط ملف.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(\"archive.tar\");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

هذا المُنشئ لا يفك أي إدخال. راجع طريقة [TarEntry.open()](../../com.aspose.zip/tarentry\\#open--) للتفكيك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


ينشئ مثيلًا جديدًا من الفئة [TarArchive](../../com.aspose.zip/tararchive) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

المثال التالي يوضح كيفية استخراج جميع العناصر إلى دليل.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | java.io.File | الدليل للضغط |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | java.lang.String | الدليل للضغط |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والدلائل بشكل تكراري في الدليل المحدد.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

يتم تعيين اسم الإدخال فقط داخل معامل `name`. اسم الملف المقدم في معامل `file` لا يؤثر على اسم الإدخال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| file | java.io.File | البيانات الوصفية للملف أو المجلد المراد ضغطه |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

```

``````

File fi = new File(\"data.bin\");
try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"data.bin\", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

اسم الإدخال يتم تعيينه فقط داخل معامل `name`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| source | java.io.InputStream | دفق الإدخال للعنصر |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"bytes\", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

يتم تعيين اسم الإدخال فقط داخل معامل `name`. اسم الملف المقدم في معامل `path` لا يؤثر على اسم الإدخال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال |
| path | java.lang.String | مسار الملف ليتم ضغطه |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | الإدخال لإزالته من قائمة الإدخالات |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


يزيل الإدخال من قائمة الإدخالات حسب الفهرس.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

إذا لم يكن الدليل موجودًا، فسيتم إنشاؤه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | مسار الدليل الذي توضع فيه الملفات المستخرجة |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


يستخرج أرشيف gzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف gzip بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج GZip غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


يستخرج أرشيف gzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف gzip بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج GZip غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الأرشيف. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


يستخرج أرشيف LZ4 المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف LZ4 بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | source | java.io.InputStream | مصدر الأرشيف. |

تدفق استخراج LZ4 غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


يستخرج أرشيف LZ4 المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف LZ4 بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | المسار إلى ملف الأرشيف. |

تدفق استخراج LZ4 غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


يستخرج أرشيف LZMA المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف LZMA بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج LZMA غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


يستخرج أرشيف LZMA المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف LZMA بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج LZMA غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


يستخرج أرشيف lzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف lzip بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج Lzip غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


يستخرج أرشيف lzip المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف lzip بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

تدفق استخراج Lzip غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار إلى ملف الأرشيف. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


يستخرج أرشيف بصيغة xz المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف xz بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


يستخرج أرشيف بصيغة xz المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف xz بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


يستخرج أرشيف بصيغة Z المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف Z بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


يستخرج أرشيف بصيغة Z المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف Z بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


يستخرج أرشيف Zstandard المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف Zstandard بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | java.io.InputStream | مصدر الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


يستخرج أرشيف Zstandard المقدم ويكوّن [TarArchive](../../com.aspose.zip/tararchive) من البيانات المستخرجة.

هام: يتم استخراج أرشيف Zstandard بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتوياته داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار ملف الأرشيف |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


يحصل على إدخالات من نوع [TarEntry](../../com.aspose.zip/tarentry) التي تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - مدخلات من نوع [TarEntry](../../com.aspose.zip/tarentry) تشكّل الأرشيف
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل أرشيف tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - مدخلات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) تشكّل أرشيف tar
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

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ الأرشيف إلى ملف الوجهة المقدم.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

من الممكن حفظ الأرشيف إلى نفس المسار الذي تم تحميله منه. ومع ذلك، لا يُنصح بذلك لأن هذه الطريقة تستخدم النسخ إلى ملف مؤقت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


يحفظ الأرشيف إلى الدفق مع ضغط gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


يحفظ الأرشيف إلى الملف بالمسار مع ضغط gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


يحفظ الأرشيف إلى الدفق باستخدام ضغط LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس ملف tar. سيتم التعامل مع القيمة الفارغة كـ USTar عندما يكون ذلك ممكنًا. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس ملف tar. سيتم التعامل مع القيمة الفارغة كـ USTar عندما يكون ذلك ممكنًا. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


يحفظ الأرشيف إلى الدفق باستخدام ضغط LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

مهم: يتم إنشاء أرشيف tar ثم ضغطه داخل هذه الدالة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

مهم: يتم إنشاء أرشيف tar ثم ضغطه داخل هذه الدالة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


يحفظ الأرشيف إلى الدفق مع ضغط lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


يحفظ الأرشيف إلى الملف بالمسار مع ضغط lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


يحفظ الأرشيف إلى الدفق مع ضغط xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output`يجب أن يكون التدفق قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


يحفظ الأرشيف إلى الدفق مع ضغط xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


يحفظ الأرشيف إلى الملف بالمسار مع ضغط xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | مجموعة من إعدادات أرشيف xz الخاصة: حجم القاموس، حجم الكتلة، نوع الفحص |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


يحفظ الأرشيف إلى الدفق مع ضغط Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| output | java.io.OutputStream | دفق الوجهة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


يحفظ الأرشيف إلى الملف بالمسار مع ضغط Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


يحفظ الأرشيف إلى الدفق مع ضغط Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلاً للكتابة |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


يحفظ الأرشيف إلى الملف بالمسار مع ضغط Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | يحدد تنسيق رأس tar. سيتم معالجة القيمة Null كـ USTar عندما يكون ذلك ممكنًا |

