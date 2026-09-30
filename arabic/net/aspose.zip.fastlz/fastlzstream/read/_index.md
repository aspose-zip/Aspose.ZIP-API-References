---
title: "FastLZStream.Read"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة FastLZStream. تقرأ تسلسلًا من البايتات من التيار وتتحرك الموضع داخل التيار بعدد البايتات المقروءة. غير مدعوم."
type: docs
weight: 90
url: /ar/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

يقرأ تسلسلًا من البايتات من التدفق ويقدم الموضع داخل التدفق بعدد البايتات المقروءة. غير مدعوم.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| buffer | Byte[] | مصفوفة من البايتات. عندما تعود هذه الطريقة، يحتوي buffer على مصفوفة البايتات المحددة مع القيم بين offset و (offset + count - 1) التي تم استبدالها بالبايتات المقروءة من المصدر الحالي. |
| offset | Int32 | الإزاحة الصفريّة للبايت في buffer التي يبدأ عندها تخزين البيانات المقروءة من التيار الحالي. |
| count | Int32 | الحد الأقصى لعدد البايتات التي ستُقرأ من التيار الحالي. |

### قيمة الإرجاع

إجمالي عدد البايتات المقروءة إلى buffer. قد يكون أقل من عدد البايتات المطلوب إذا لم تتوفر تلك البايتات حاليًا، أو صفر (0) إذا تم الوصول إلى نهاية التيار.

### استثناءات

| استثناء | شرط |
| --- | --- |
| NotSupportedException | العملية غير مدعومة. |

### انظر أيضًا

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


