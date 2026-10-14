---
title: "XarArchive.CreateEntries"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة XarArchive. تضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المحدد"
type: docs
weight: 30
url: /ar/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

تضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المحدد.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | String | الدليل للضغط. |
| compressionSettings | Boolean | إعدادات الضغط المستخدمة للعناصر المضافة [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | يشير إلى ما إذا كان يجب تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *sourceDirectory* فارغ. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول إلى *sourceDirectory*. |
| ArgumentException | *sourceDirectory* يحتوي على أحرف غير صالحة مثل ", &lt;, &gt;, أو &#x7C;. |
| PathTooLongException | المسار المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. المسار المحدد، أو اسم الملف، أو كلاهما طويل جدًا. |
| IOException | *sourceDirectory* يمثل ملفًا، وليس دليلًا. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### انظر أيضًا

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

تضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المحدد.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | DirectoryInfo | الدليل للضغط. |
| compressionSettings | Boolean | إعدادات الضغط المستخدمة للعناصر المضافة [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | يشير إلى ما إذا كان يجب تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *directory* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول إلى *directory*. |
| IOException | *directory* يمثل ملفًا، وليس دليلًا. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### انظر أيضًا

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


