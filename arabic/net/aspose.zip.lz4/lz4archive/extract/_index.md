---
title: "Lz4Archive.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة Lz4Archive. تستخرج الأرشيف إلى الملف حسب المسار"
type: docs
weight: 30
url: /ar/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

يستخرج الأرشيف إلى الملف حسب المسار.

```csharp
public FileInfo Extract(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |

### قيمة الإرجاع

معلومات ملف مستخرج.

### استثناءات

| استثناء | شرط |
| --- | --- |
| EndOfStreamException | تدفق المصدر قصير جدًا. |
| InvalidDataException | تم العثور على بايتات خاطئة أثناء فك الترميز. |
| NotSupportedException | إصدار LZ4 هذا غير مدعوم. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | تم إعداد الأرشيف للتركيب. |

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

يستخرج الأرشيف إلى الدفق المقدم.

```csharp
public void Extract(Stream destination)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | تيار | دفق الوجهة. يجب أن يكون قابلًا للكتابة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | *destination* لا يدعم الكتابة. |
| EndOfStreamException | تدفق المصدر قصير جدًا. |
| InvalidDataException | تم العثور على بايتات خاطئة أثناء فك الترميز. |
| NotSupportedException | إصدار LZ4 هذا غير مدعوم. |
| InvalidOperationException | تم إعداد الأرشيف للتركيب. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


