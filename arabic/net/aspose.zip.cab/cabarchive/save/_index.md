---
title: "CabArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة CabArchive. تحفظ الأرشيف إلى الدفق المقدم."
type: docs
weight: 70
url: /ar/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| outputStream | تيار | دفق الوجهة. |
| saveOptions | CabSaveOptions | خيارات حفظ الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | *outputStream* غير قابل للكتابة ولا قابل للتمرير. |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكن حفظه. |

## ملاحظات

*outputStream* must be writable.

## أمثلة

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### انظر أيضًا

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

يحفظ الأرشيف إلى ملف الوجهة المحدد.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| saveOptions | CabSaveOptions | خيارات حفظ الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *destinationFileName* هو null. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | الـ *destinationFileName* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *destinationFileName*. |
| PathTooLongException | الـ *destinationFileName* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *destinationFileName* يحتوي على نقطتين (:) في وسط السلسلة. |
| FileNotFoundException | الملف غير موجود. |
| InvalidOperationException | تم فتح الأرشيف للاستخراج. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

يمكن حفظ الأرشيف إلى نفس المسار الذي تم تحميله منه. ومع ذلك، لا يُنصح بذلك لأن هذه الطريقة تستخدم النسخ إلى ملف مؤقت.

## أمثلة

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### انظر أيضًا

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


