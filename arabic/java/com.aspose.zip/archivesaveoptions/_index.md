---
title: "ArchiveSaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات حفظ أرشيف ZIP."
type: docs
weight: 36
url: /ar/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

خيارات حفظ أرشيف ZIP.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | يحصل على التعليق الاختياري لملف Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | يحصل على قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرة بعد ضغط الإدخال. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | يحصل على إعدادات إصدار وصف البيانات. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات. |
| [getEncryptionOptions()](#getEncryptionOptions--) | يحصل على إعدادات التشفير لحفظ أرشيف ZIP الموجود. |
| [getEventsBag()](#getEventsBag--) | يحصل على حاوية الأحداث التي تُثار عند حفظ الأرشيف. |
| [getParallelOptions()](#getParallelOptions--) | يحصل على إعدادات الضغط المتوازي. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | يحصل على إعدادات الأرشيف القابل للاستخراج الذاتي. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | يضبط التعليق الاختياري لملف Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرةً بعد ضغط الإدخال. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | يضبط إعدادات لإصدار موصّف البيانات. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | يضبط إعدادات التشفير لحفظ أرشيف ZIP الموجود. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | يضبط حاوية الأحداث التي تُثار عند حفظ الأرشيف. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | يضبط إعدادات الضغط المتوازي. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | يضبط إعدادات الأرشيف المستخرج ذاتيًا. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


يحصل على التعليق الاختياري لملف Zip.

**Returns:**
java.lang.String - تعليق اختياري لملف Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرة بعد ضغط الإدخال.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرةً بعد ضغط الإدخال.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


يحصل على إعدادات إصدار وصف البيانات.

الخيار الافتراضي هو دائمًا موصّف البيانات الموجود.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات.

إذا لم يتم ضبطه، سيتم استخدام صفحة الشيفرة 437.

**Returns:**
java.nio.charset.Charset - الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


يحصل على إعدادات التشفير لحفظ أرشيف ZIP الموجود.

```

``````

try (Archive archive = new Archive("plain.zip")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
archive.save("encripted.zip", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

لا تستخدم هذه الخيارات لإنشاء أرشيف مشفر بشكل عادي، استخدم

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) بدلاً من ذلك.

غير متوافق مع `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) ذات القيمة [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | من إعدادات تشفير الحفظ لأرشيف ZIP الموجود. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


يضبط حاوية الأحداث التي تُثار عند حفظ الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | حاوية الأحداث التي تُرفع عند حفظ الأرشيف. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


يضبط إعدادات الضغط المتوازي.

قم بتعيينه إذا كنت تريد استخدام عدة نوى CPU أثناء ضغط عدة مدخلات أرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | إعدادات الضغط المتوازي. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


يضبط إعدادات الأرشيف المستخرج ذاتيًا.

قم بتعيينه إذا كنت بحاجة إلى إنشاء برنامج قابل للتنفيذ لاستخراج أرشيف دون أي برنامج مثبت على الحاسوب الهدف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | إعدادات الأرشيف المستخرج ذاتيًا. |

