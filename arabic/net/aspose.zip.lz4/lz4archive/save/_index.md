---
title: "Lz4Archive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة Lz4Archive. تحفظ أرشيف lz4 إلى الدفق المقدم"
type: docs
weight: 60
url: /ar/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

يحفظ أرشيف lz4 إلى التدفق المحدد.

```csharp
public void Save(Stream output)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *output* فارغ. |
| ArgumentException | *output* غير قابل للكتابة. |
| InvalidOperationException | الأرشيف مُجهز للاستخراج. - أو - لم يتم توفير المصدر. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يُرمى عندما يتم إلغاء الضغط عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

*output* must be seekable.

## أمثلة

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

يحفظ أرشيف lz4 إلى ملف الوجهة المحدد.

```csharp
public void Save(FileInfo destination)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | FileInfo | FileInfo، الذي سيفتح كدفق وجهة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب لفتح *destination*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات فقط. |
| FileNotFoundException | الملف غير موجود. |
| UnauthorizedAccessException | المسار إلى الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *destination* فارغ. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| InvalidOperationException | تم إعداد الأرشيف للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

يحفظ الأرشيف إلى ملف الوجهة المحدد.

```csharp
public void Save(string destinationFileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *destinationFileName* هو null. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول |
| ArgumentException | الـ *destinationFileName* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *destinationFileName*. |
| PathTooLongException | الـ *destinationFileName* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *destinationFileName* يحتوي على نقطتين (:) في وسط السلسلة. |
| InvalidOperationException | تم إعداد الأرشيف للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| DirectoryNotFoundException | المسار المحدد غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| FileNotFoundException | الملف المحدد في *destinationFileName* لم يُعثر عليه. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |

## أمثلة

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


