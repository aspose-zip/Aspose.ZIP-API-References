---
title: "ZstandardArchive.Open"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة ZstandardArchive. يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف"
type: docs
weight: 50
url: /ar/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

يفتح الأرشيف للاستخراج ويوفر تدفقاً بمحتوى الأرشيف.

```csharp
public Stream Open()
```

### قيمة الإرجاع

التدفق الذي يمثل محتويات الأرشيف.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

## أمثلة

يستخرج الأرشيف وينسخ المحتوى المستخرج إلى تدفق الملف.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

يمكنك استخدام طريقة Stream.CopyTo لـ .NET 4.0 وما فوق:

```csharp
unpacked.CopyTo(extracted);
```

### انظر أيضًا

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


