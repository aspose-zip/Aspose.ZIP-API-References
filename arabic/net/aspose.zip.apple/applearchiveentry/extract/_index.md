---
title: "AppleArchiveEntry.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة AppleArchiveEntry. تستخرج الإدخال إلى نظام الملفات بالمسار المقدم"
type: docs
weight: 50
url: /ar/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم.

```csharp
public FileInfo Extract(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidDataException | المجموع الاختباري أو البصمة المخزنة للمدخل لا تتطابق مع البيانات المستخرجة. |
| InvalidOperationException | المدخل ينتمي إلى أرشيف مُعد للتكوين، أو لا يمكن فتح بيانات المدخل من تدفق أرشيف غير قابل للتمرير. |
| NotSupportedException | المدخل ينتمي إلى أرشيف Apple صلب أو يستخدم طريقة ضغط غير مدعومة. |
| ObjectDisposedException | تم التخلص من تدفق المصدر. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

### انظر أيضًا

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
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
| ArgumentNullException | *destination* هو `null`. |
| ArgumentException | *destination* لا يدعم الكتابة. |
| InvalidDataException | المجموع الاختباري أو البصمة المخزنة للمدخل لا تتطابق مع البيانات المستخرجة. |
| InvalidOperationException | المدخل ينتمي إلى أرشيف مُعد للتكوين، أو لا يمكن فتح بيانات المدخل من تدفق أرشيف غير قابل للتمرير. |
| NotSupportedException | المدخل ينتمي إلى أرشيف Apple صلب أو يستخدم طريقة ضغط غير مدعومة. |
| ObjectDisposedException | تم التخلص من تدفق المصدر. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

### انظر أيضًا

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


