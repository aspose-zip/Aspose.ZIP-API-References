---
title: "AppleArchiveEntry.Open"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة AppleArchiveEntry. يفتح المدخل للاستخراج ويوفر تدفقًا بمحتوى المدخل"
type: docs
weight: 60
url: /ar/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال.

```csharp
public Stream Open()
```

### قيمة الإرجاع

تدفق قابل للقراءة يحتوي على بيانات المدخل المستخرجة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| NotSupportedException | المدخل ينتمي إلى أرشيف Apple صلب أو يستخدم طريقة ضغط غير مدعومة. |
| InvalidDataException | المجموع الاختباري أو البصمة المخزنة للمدخل لا تتطابق مع البيانات المستخرجة. |
| InvalidOperationException | المدخل ينتمي إلى أرشيف مُعد للتكوين، أو لا يمكن فتح بيانات المدخل من تدفق أرشيف غير قابل للتمرير. |
| ObjectDisposedException | تم التخلص من تدفق المصدر. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

اقرأ من التدفق المعاد للحصول على محتوى المدخل الأصلي. إذا كان الأرشيف يحتوي على حقول المجموع الاختباري، يتم التحقق من المجموع الاختباري أثناء قراءة التدفق المعاد.

### انظر أيضًا

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


