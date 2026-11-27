---
title: "SplitArchiveSaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات حفظ أرشيف ZIP متعدد الأحجام."
type: docs
weight: 122
url: /ar/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

خيارات حفظ أرشيف ZIP متعدد الأحجام.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | ينشئ إعدادات لحفظ أرشيف ZIP متعدد الأحجام. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | يحصل على التعليق الاختياري لملف Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | يحصل على قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرة بعد ضغط الإدخال. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات. |
| [getEventsBag()](#getEventsBag--) | يحصل على حاوية الأحداث التي تُثار عند حفظ الأرشيف. |
| [getFileName()](#getFileName--) | يحصل على اسم الأجزاء دون الامتداد. |
| [getSegmentSize()](#getSegmentSize--) | يحصل على حجم الجزء. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | يضبط التعليق الاختياري لملف Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرةً بعد ضغط الإدخال. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | يضبط حاوية الأحداث التي تُثار عند حفظ الأرشيف. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


ينشئ إعدادات لحفظ أرشيف ZIP متعدد الأحجام.

قد تكون بعض الأحجام أقل من `segmentSize`. في معظم الحالات، سيكون الجزء الأخير أصغر، لكن نادراً ما قد تكون الأجزاء العادية أكبر من ذلك.

ستكون أسماء الملفات كما يلي: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الأحجام. قد يكون مع أو بدون امتداد .zip. |
| segmentSize | long | حجم الجزء. |

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
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات.

إذا لم يتم ضبطه، سيتم استخدام صفحة الشيفرة 437.

**Returns:**
java.nio.charset.Charset - الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


يحصل على حاوية الأحداث التي تُثار عند حفظ الأرشيف.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


يحصل على اسم الأجزاء دون الامتداد.

**Returns:**
java.lang.String - اسم الأجزاء دون الامتداد.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


يحصل على حجم الجزء.

**Returns:**
long - حجم الجزء.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


يضبط التعليق الاختياري لملف Zip.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.lang.String | تعليق اختياري لملف Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرةً بعد ضغط الإدخال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كان يجب إغلاق مصادر الإدخالات مباشرةً بعد ضغط الإدخال. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


يضبط الترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات.

إذا لم يتم ضبطه، سيتم استخدام صفحة الشيفرة 437.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.nio.charset.Charset | ترميز لتحويل أسماء الملفات والسلاسل الأخرى إلى بايتات. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


يضبط حاوية الأحداث التي تُثار عند حفظ الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | حاوية الأحداث التي تُرفع عند حفظ الأرشيف. |

