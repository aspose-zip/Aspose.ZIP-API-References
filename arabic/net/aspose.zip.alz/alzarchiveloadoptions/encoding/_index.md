---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية AlzArchiveLoadOptions. تُحصل أو تُعيّن الترميز لأسماء الإدخالات. القيمة الافتراضية هي صفحة الشيفرة الكورية لنظام ويندوز 949 CP949"
type: docs
weight: 40
url: /ar/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

يحصل أو يضبط الترميز لأسماء الإدخالات. القيمة الافتراضية هي صفحة الترميز الكورية لنظام ويندوز 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## ملاحظات

تخزن أرشيفات ALZ تاريخيًا أسماء الملفات باستخدام صفحة الشيفرة ANSI لنظام ويندوز الكوري.

## أمثلة

اسم الإدخال مُكوّن باستخدام الترميز المحدد.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### انظر أيضًا

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


