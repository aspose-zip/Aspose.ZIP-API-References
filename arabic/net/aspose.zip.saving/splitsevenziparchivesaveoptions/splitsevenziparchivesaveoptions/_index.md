---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP لمرجع .NET API
description: SplitSevenZipArchiveSaveOptions البناء. يثبّت الإعدادات لحفظ أرشيف 7z متعدد المجلدات.
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

يثبّت الإعدادات لحفظ أرشيف 7z متعدد المجلدات.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | اسم المجلدات. قد يكون بامتداد .7z أو بدونه. |
| segmentSize | UInt32 | حجم الحجم. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* أقل من 100. |

### ملاحظات

قد تكون بعض الأحجام أقل من*segmentSize*. في معظم الحالات ، سيكون الجزء الأخير أقل ولكن نادرًا ما تكون الشرائح العادية أيضًا.

ستكون أسماء الملفات على النحو التالي:*fileName* .7z.001 ،*fileName* .7z.002، ...،*fileName*.7z. (اسم).

### أنظر أيضا

* class [SplitSevenZipArchiveSaveOptions](../)
* مساحة الاسم [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* المجسم [Aspose.Zip](../../../)


