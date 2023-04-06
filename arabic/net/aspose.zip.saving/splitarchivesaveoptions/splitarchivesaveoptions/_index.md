---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP لمرجع .NET API
description: SplitArchiveSaveOptions البناء. يتم إنشاء إعدادات لحفظ أرشيف مضغوط متعدد المجلدات.
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

يتم إنشاء إعدادات لحفظ أرشيف مضغوط متعدد المجلدات.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | اسم المجلدات. قد يكون بامتداد .zip أو بدونه. |
| segmentSize | UInt32 | حجم الحجم. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | حجم المقطع أقل من 65536 بايت. |

### ملاحظات

قد تكون بعض الأحجام أقل من*segmentSize*. في معظم الحالات ، سيكون الجزء الأخير أقل ولكن نادرًا ما تكون الشرائح العادية أيضًا.

ستكون أسماء الملفات على النحو التالي:*fileName* .z01 ،*fileName* .z02، ...،*fileName* .z (ن -1) ،*fileName*.أَزِيز.

### أنظر أيضا

* class [SplitArchiveSaveOptions](../)
* مساحة الاسم [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* المجسم [Aspose.Zip](../../../)


