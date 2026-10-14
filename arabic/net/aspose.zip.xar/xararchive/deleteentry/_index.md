---
title: "XarArchive.DeleteEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة XarArchive. تزيل الظهور الأول لمدخل محدد من قائمة المدخلات"
type: docs
weight: 50
url: /ar/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

تزيل الظهور الأول لمدخل محدد من قائمة المدخلات.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مدخل | XarEntry | المدخل الذي سيُزال من قائمة المدخلات. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *entry* هو null. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | الأرشيف غير مفتوح للاستخراج. |

## أمثلة

إليك كيفية إزالة جميع المدخلات باستثناء الأخير:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### انظر أيضًا

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


