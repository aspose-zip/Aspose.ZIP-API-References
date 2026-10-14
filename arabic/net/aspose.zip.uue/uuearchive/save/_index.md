---
title: "UueArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة UueArchive. يحفظ الأرشيف إلى الدفق المقدم"
type: docs
weight: 70
url: /ar/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| outputStream | تيار | دفق الوجهة. |
| saveOptions | UueSaveOptions | خيارات حفظ الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | لم يتم توفير مصدر البيانات المراد أرشفته. |
| ArgumentException | *outputStream* غير قابل للكتابة. |
| UnauthorizedAccessException | مصدر الملف للقراءة فقط أو أنه دليل. |
| DirectoryNotFoundException | مسار مصدر الملف المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | مصدر الملف مفتوح بالفعل. |

## ملاحظات

*outputStream* must be writable.

## أمثلة

اكتب البيانات المضغوطة إلى دفق استجابة http.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### انظر أيضًا

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

يحفظ الأرشيف إلى ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| saveOptions | UueSaveOptions | خيارات حفظ الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | *destinationFileName* هو null. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | الـ *destinationFileName* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *destinationFileName*. |
| PathTooLongException | الـ *destinationFileName* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *destinationFileName* يحتوي على نقطتين (:) في وسط السلسلة. |
| InvalidOperationException | لم يتم توفير مصدر البيانات المراد أرشفته. |

## أمثلة

اكتب البيانات المشفرة إلى الملف.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### انظر أيضًا

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


