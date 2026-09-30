---
title: "XarArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة XarArchive. تحفظ الأرشيف إلى ملف الوجهة المحدد."
type: docs
weight: 80
url: /ar/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

يحفظ الأرشيف إلى ملف الوجهة المحدد.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| saveOptions | XarSaveOptions | خيارات لحفظ أرشيف xar. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *destinationFileName* هو null. |
| InvalidOperationException | من المستحيل تعديل أرشيف xar. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. |
| UnauthorizedAccessException | *destinationFileName* يشير إلى ملف للقراءة فقط. - أو - *destinationFileName* يشير إلى دليل. - أو - المستدعي لا يملك الإذن المطلوب. |

### انظر أيضًا

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |
| saveOptions | XarSaveOptions | خيارات لحفظ أرشيف xar. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *output* فارغ. |
| ArgumentException | *output* غير قابل للكتابة/القراءة أو غير قابل للتمرير. |
| InvalidOperationException | من المستحيل تعديل أرشيف xar. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

### انظر أيضًا

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


