---
title: "ZstandardArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة ZstandardArchive. تحفظ الأرشيف إلى الدفق المقدم"
type: docs
weight: 60
url: /ar/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| outputStream | تيار | دفق الوجهة. |
| الإعدادات | ZstandardSaveOptions | إعدادات اختيارية لتكوين الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentException | *outputStream* غير قابل للكتابة. |
| InvalidOperationException | لم يتم توفير المصدر. |

## ملاحظات

*outputStream* must be writable.

## أمثلة

اكتب البيانات المضغوطة إلى دفق استجابة http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### انظر أيضًا

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

يحفظ الأرشيف إلى ملف الوجهة المحدد.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| الإعدادات | ZstandardSaveOptions | إعدادات اختيارية لتكوين الأرشيف. |

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
| استثناء | يُرمى عندما يحدث خطأ في وقت التشغيل. |
| DirectoryNotFoundException | المسار المحدد غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |
| InvalidOperationException | لم يتم توفير المصدر. |

## أمثلة

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### انظر أيضًا

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

يحفظ الأرشيف إلى ملف الوجهة المحدد.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | FileInfo | FileInfo، الذي سيفتح كدفق وجهة. |
| الإعدادات | ZstandardSaveOptions | إعدادات اختيارية لتكوين الأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب لفتح *destination*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات فقط. |
| FileNotFoundException | الملف غير موجود. |
| UnauthorizedAccessException | المسار إلى الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *destination* فارغ. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| InvalidOperationException | لم يتم توفير المصدر. |

## أمثلة

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### انظر أيضًا

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


