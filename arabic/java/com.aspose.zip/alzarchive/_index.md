---
title: "AlzArchive"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "يمثل ملف أرشيف ALZ."
type: docs
weight: 11
url: /ar/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

يمثل ملف أرشيف ALZ. استخدم هذه الفئة لفحص واستخراج أرشيفات ALZ.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | يُهيئ أرشيف ALZ من تدفق. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | يُهيئ أرشيف ALZ من تدفق باستخدام خيارات التحميل المقدمة. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | يُهيئ أرشيف ALZ من مسار ملف. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | يُهيئ أرشيف ALZ من مسار ملف باستخدام خيارات التحميل المقدمة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | يطلق الموارد التي يحتفظ بها هذا الأرشيف. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات والأدلة إلى الدليل المقدم. |
| [getEntries()](#getEntries--) | يحصل على الإدخالات التي تشكل هذا الأرشيف. |
| [getFileEntries()](#getFileEntries--) | يحصل على الإدخالات عبر واجهة الأرشيف العامة. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الأرشيف. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


يُهيئ أرشيف ALZ من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | تدفق أرشيف ALZ؛ يجب أن يدعم القراءة والبحث |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


يُهيئ أرشيف ALZ من تدفق باستخدام خيارات التحميل المقدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.InputStream | تدفق أرشيف ALZ؛ يجب أن يدعم القراءة والبحث |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | الخيارات المستخدمة لتحميل الأرشيف |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


يُهيئ أرشيف ALZ من مسار ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مسار الملف | java.lang.String | مسار إلى أرشيف ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


يُهيئ أرشيف ALZ من مسار ملف باستخدام خيارات التحميل المقدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مسار الملف | java.lang.String | مسار إلى أرشيف ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | الخيارات المستخدمة لتحميل الأرشيف |

### close() {#close--}
```
public void close()
```


يطلق الموارد التي يحتفظ بها هذا الأرشيف.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات والأدلة إلى الدليل المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دليل الوجهة | java.lang.String | دليل الوجهة؛ يتم إنشاؤه عند الحاجة |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


يحصل على الإدخالات التي تشكل هذا الأرشيف.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - قائمة ثابتة من إدخالات ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


يحصل على الإدخالات عبر واجهة الأرشيف العامة.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - إدخالات الأرشيف
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


يحصل على تنسيق الأرشيف.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
