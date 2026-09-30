---
title: "LzxArchiveEntry.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة LzxArchiveEntry. تستخرج مدخل أرشيف Lzx إلى نظام ملفات حسب المسار"
type: docs
weight: 80
url: /ar/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

يستخرج إدخال أرشيف Lzx إلى نظام ملفات حسب المسار.

```csharp
public FileSystemInfo Extract(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى الملف الذي سيخزن البيانات غير المضغوطة. |

### قيمة الإرجاع

FileSystemInfoInstance يحتوي على البيانات المستخرجة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| NotSupportedException | طريقة ضغط غير صالحة. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |

## أمثلة

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### انظر أيضًا

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

يستخرج الإدخال إلى الدفق المقدم.

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
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| ArgumentNullException | دفق الوجهة هو null. |
| NotSupportedException | طريقة ضغط غير صالحة. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |

### انظر أيضًا

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


