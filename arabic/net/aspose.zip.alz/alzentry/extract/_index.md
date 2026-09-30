---
title: "AlzEntry.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة AlzEntry. تستخرج العنصر إلى نظام الملفات باستخدام المسار المقدم"
type: docs
weight: 60
url: /ar/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم.

```csharp
public FileInfo Extract(string path, string password = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |
| كلمة المرور | String | كلمة مرور اختيارية لفك التشفير. |

### قيمة الإرجاع

معلومات الملف لملف مركب.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| InvalidDataException | الأرشيف تالف. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| FileNotFoundException | الملف غير موجود. |

## أمثلة

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### انظر أيضًا

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

يستخرج الإدخال إلى الدفق المقدم.

```csharp
public void Extract(Stream destination, string password = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | تيار | دفق الوجهة. يجب أن يكون قابلًا للكتابة. |
| كلمة المرور | String | كلمة مرور اختيارية لفك التشفير. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | *destination* لا يدعم الكتابة. |
| InvalidOperationException | الأرشيف غير مفتوح للاستخراج. - أو - هذا العنصر هو دليل. |
| InvalidDataException | بيانات خاطئة داخل العنصر. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |

## أمثلة

استخراج عنصر من أرشيف ALZ باستخدام كلمة المرور.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### انظر أيضًا

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


