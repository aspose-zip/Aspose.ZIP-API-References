---
title: "SevenZipEntrySettings.Solid"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية SevenZipEntrySettings. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب ربط الإدخالات ومعاملتها ككتلة بيانات واحدة"
type: docs
weight: 50
url: /ar/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

يحصل أو يضبط القيمة التي تشير إلى ما إذا كان يجب دمج الإدخالات ومعاملتها ككتلة بيانات واحدة.

```csharp
public bool Solid { get; set; }
```

## ملاحظات

قدّم `SevenZipEntrySettings` لأرشيف 7z الصلب عند إنشاء الأرشيف.

## أمثلة

المثال التالي يوضح كيفية ضغط دليل إلى أرشيف 7z صلب باستخدام ضغط LZMA2 دون تشفير.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### انظر أيضًا

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


