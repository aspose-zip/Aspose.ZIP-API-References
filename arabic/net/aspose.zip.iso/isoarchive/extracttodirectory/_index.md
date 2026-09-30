---
title: "IsoArchive.ExtractToDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة IsoArchive. تستخرج جميع الإدخالات إلى الدليل المحدد"
type: docs
weight: 60
url: /ar/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

يستخرج جميع الإدخالات إلى الدليل المحدد.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationDirectory | String | الدليل لاستخراج الإدخالات إليه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يتم إلقاء الاستثناء عندما يكون الأرشيف في وضع التحرير. |
| ArgumentNullException | يتم إلقاء الاستثناء عندما يكون *destinationDirectory* فارغًا. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى دليل:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### انظر أيضًا

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


