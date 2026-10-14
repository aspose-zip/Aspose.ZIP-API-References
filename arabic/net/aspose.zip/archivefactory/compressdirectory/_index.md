---
title: "ArchiveFactory.CompressDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة ArchiveFactory. تضغط الدليل المحدد إلى ملف أرشيف باستخدام تنسيق الأرشيف المقدم"
type: docs
weight: 10
url: /ar/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

يضغط الدليل المحدد إلى ملف أرشيف باستخدام تنسيق الأرشيف المقدم.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى الدليل الذي سيتم ضغطه. |
| outputFileName | String | اسم ملف الوجهة. |
| archiveFormat | ArchiveFormat | تنسيق الأرشيف لإنشائه (مثال: zip، rar، tar، إلخ). |

### استثناءات

| استثناء | شرط |
| --- | --- |
| DirectoryNotFoundException | يُرمى إذا كان الدليل المحدد بواسطة *path* غير موجود. |
| ArgumentException | يُرمى إذا كان *path* null أو سلسلة فارغة. |
| NotSupportedException | يُرمى إذا كان *archiveFormat* المحدد غير مدعوم أو غير معروف. |
| ArgumentNullException | *path* هو `null`. |

## ملاحظات

ستقوم هذه الطريقة بإنشاء ملف أرشيف في الموقع المحدد بواسطة معامل *path*. عادةً ما يكون اسم ملف الأرشيف هو اسم الدليل متبوعًا بامتداد الملف المناسب بناءً على *archiveFormat*. الدليل نفسه لا يتم تعديله أو حذفه.

## أمثلة

فيما يلي مثال على كيفية استخدام طريقة CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// سيتم إنشاء ملف ZIP بمحتويات الدليل في المسار المحدد.
```

### انظر أيضًا

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


