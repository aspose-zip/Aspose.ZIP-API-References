---
title: "GzipArchive.UncompressedSize"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية GzipArchive. تحصل على حجم الملف الأصلي."
type: docs
weight: 30
url: /ar/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

يحصل على حجم ملف أصلي.

```csharp
public ulong UncompressedSize { get; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

أثناء فك الضغط، قد تحتوي هذه الخاصية على حجم غير صحيح. إذا تجاوز حجم الملف غير المضغوط 4 جيجابايت، ستعطي هذه الخاصية قيمة خاطئة بسبب حد 32 بت في الرأس.

### انظر أيضًا

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


