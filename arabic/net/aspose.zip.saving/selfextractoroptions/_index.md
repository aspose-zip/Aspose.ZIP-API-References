---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Saving.SelfExtractorOptions فصل. خيارات لإنشاء أرشيف قابل للتنفيذ يتم استخراجه ذاتيًا.
type: docs
weight: 500
url: /ar/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

خيارات لإنشاء أرشيف قابل للتنفيذ يتم استخراجه ذاتيًا.

```csharp
public class SelfExtractorOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب إغلاق نافذة المستخرج عند الاستخراج أم لا. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | الحصول على عنوان نافذة المستخرج أو تحديده. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | الحصول على أو تعيين برنامج ليتم تنفيذه بعد اكتمال استخراج الأرشيف. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | الحصول على أو تعيين رمز المسار إلى العنوان للنوافذ الرئيسية لتطبيق المستخرج. |

### ملاحظات

لا يمكن تكوين أرشيف يتم استخراجه ذاتيًا بترخيص مقنن:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### أمثلة

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### أنظر أيضا

* مساحة الاسم [Aspose.Zip.Saving](../../aspose.zip.saving/)
* المجسم [Aspose.Zip](../../)


