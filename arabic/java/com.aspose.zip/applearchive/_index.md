---
title: "AppleArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "هذه الفئة تمثل ملف Apple Archive بامتداد .aar."
type: docs
weight: 16
url: /ar/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

هذه الفئة تمثل ملف Apple Archive (.aar). استخدمها لإنشاء ملفات Apple Archive.

Apple و Apple Archive هما علامتا تجاريتان لشركة Apple Inc.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) مع الإعدادات المستخدمة للمدخلات المُكوّنة. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) مع الإعدادات المستخدمة للمدخلات المُكوّنة. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر داخل الدليل المحدد. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر داخل الدليل المحدد. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | ينشئ إدخالاً واحداً داخل الأرشيف. |
| [dispose()](#dispose--) | ينفذ مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد. |
| [getEntries()](#getEntries--) | يحصل على المدخلات التي تشكل الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
| [getNewEntrySettings()](#getNewEntrySettings--) | يحصل على الإعدادات المستخدمة للمدخلات المُكوّنة حديثاً. |
| [isSolid()](#isSolid--) | يحصل على قيمة تشير إلى ما إذا كان الأرشيف يستخدم ضغطًا صلبًا. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ الأرشيف إلى الدفق المقدم. |
| [save(String destinationFileName)](#save-java.lang.String-) | يحفظ الأرشيف إلى ملف الوجهة المحدد. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) مع الإعدادات المستخدمة للمدخلات المُكوّنة.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) مع الإعدادات المستخدمة للمدخلات المُكوّنة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | الإعدادات المستخدمة عند إنشاء Apple Archive جديد. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | مصدر الأرشيف. |

هذا المُنشئ لا يفك ضغط أي مدخل. راجع طرق [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) و [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) لفك الضغط. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | java.io.InputStream | مصدر الأرشيف. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | خيارات لتحميل الأرشيف الموجود. |

هذا المُنشئ لا يفك ضغط أي مدخل. راجع طرق [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) و [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) لفك الضغط. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | المسار المؤهل بالكامل أو المسار النسبي لملف الأرشيف. |

هذا المُنشئ لا يفك ضغط أي مدخل. راجع طرق [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) و [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) لفك الضغط. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


ينشئ مثيلاً جديداً من الفئة [AppleArchive](../../com.aspose.zip/applearchive) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | المسار المؤهل بالكامل أو المسار النسبي لملف الأرشيف. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | خيارات لتحميل الأرشيف الموجود. |

هذا المُنشئ لا يفك ضغط أي مدخل. راجع طرق [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) و [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) لفك الضغط. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر داخل الدليل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | java.io.File | الدليل المراد ضغطه. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر داخل الدليل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | java.io.File | الدليل المراد ضغطه. |
| includeRootDirectory | boolean | يشير إلى ما إذا كان يجب تضمين الدليل الجذر نفسه أم لا. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال. |
| fileInfo | java.io.File | البيانات الوصفية للملف الذي سيتم ضغطه. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال. |
| fileInfo | java.io.File | البيانات الوصفية للملف الذي سيتم ضغطه. |
| openImmediately | boolean | صحيح إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال. |
| source | java.io.InputStream | دفق الإدخال للإدخال. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال. |
| path | java.lang.String | المسار إلى الملف المراد ضغطه. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


ينشئ إدخالاً واحداً داخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String | اسم الإدخال. |
| path | java.lang.String | المسار إلى الملف المراد ضغطه. |
| openImmediately | boolean | صحيح إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


ينفذ مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


يحصل على المدخلات التي تشكل الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - المدخلات التي تشكل الأرشيف.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات من نوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - عناصر من النوع [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) التي تشكل الأرشيف
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


يحصل على الإعدادات المستخدمة للمدخلات المُكوّنة حديثاً.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


يحصل على قيمة تشير إلى ما إذا كان الأرشيف يستخدم ضغطًا صلبًا. في الوضع الصلب، يتم ضغط جميع بيانات الإدخالات كتيار واحد ولا يتوفر استخراج إدخال فردي. استخدم [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) بدلاً من ذلك.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان الأرشيف يستخدم ضغطًا صلبًا.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


يحفظ الأرشيف إلى الدفق المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | دفق الوجهة. |

`output` يجب أن يكون قابلًا للكتابة. بعض إعدادات الضغط، مثل LZ4، تتطلب أيضًا تدفقًا قابلًا للتمرير. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


يحفظ الأرشيف إلى ملف الوجهة المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | java.lang.String | مسار الأرشيف الذي سيتم إنشاؤه. |

