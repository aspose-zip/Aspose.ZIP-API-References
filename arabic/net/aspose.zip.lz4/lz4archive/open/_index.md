---
title: "Lz4Archive.Open"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة Lz4Archive. يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف"
type: docs
weight: 50
url: /ar/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

يفتح الأرشيف للاستخراج ويوفر تدفقاً بمحتوى الأرشيف.

```csharp
public Stream Open()
```

### قيمة الإرجاع

التدفق الذي يمثل محتويات الأرشيف.

### استثناءات

| استثناء | شرط |
| --- | --- |
| EndOfStreamException | تدفق المصدر قصير جدًا. |
| InvalidDataException | تم العثور على بايتات خاطئة أثناء تهيئة فك الترميز. |
| InvalidOperationException | تم إعداد الأرشيف للتركيب. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

اقرأ من الدفق للحصول على المحتوى الأصلي للملف. راجع قسم الأمثلة.

## أمثلة

يستخرج الأرشيف وينسخ المحتوى المستخرج إلى تدفق الملف.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
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

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


