---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات حفظ أرشيف 7-zip متعدد الأحجام."
type: docs
weight: 123
url: /ar/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

خيارات حفظ أرشيف 7-zip متعدد الأحجام.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | ينشئ إعدادات لحفظ أرشيف 7z متعدد الأحجام. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFileName()](#getFileName--) | يحصل على اسم الأجزاء دون الامتداد. |
| [getSegmentSize()](#getSegmentSize--) | يحصل على حجم الجزء. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


ينشئ إعدادات لحفظ أرشيف 7z متعدد الأحجام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | fileName | java.lang.String | اسم للأحجام. قد يكون مع أو بدون امتداد .7z. |

أسماء الملفات ستكون كما يلي: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | حجم الجزء. |

قد تكون بعض الأجزاء أصغر من `segmentSize`. في معظم الحالات، سيكون الجزء الأخير أصغر لكن نادراً ما قد تكون الأجزاء العادية أكبر من ذلك. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


يحصل على اسم الأجزاء دون الامتداد.

**Returns:**
java.lang.String - اسم الأجزاء بدون امتداد
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


يحصل على حجم الجزء.

**Returns:**
long - حجم الجزء.
