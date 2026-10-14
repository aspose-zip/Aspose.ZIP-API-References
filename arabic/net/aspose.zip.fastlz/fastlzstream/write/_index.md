---
title: "FastLZStream.Write"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة FastLZStream. تكتب تسلسلًا من البايتات إلى التيار المضغوط وتتحرك الموضع الحالي داخل هذا التيار بعدد البايتات المكتوبة."
type: docs
weight: 120
url: /ar/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

يكتب تسلسلًا من البايتات إلى التدفق الضاغط ويقدم الموضع الحالي داخل هذا التدفق بعدد البايتات المكتوبة.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| buffer | Byte[] | مصفوفة من البايتات. تقوم هذه الطريقة بنسخ count بايت من buffer إلى التيار الحالي. |
| offset | Int32 | الإزاحة الصفريّة للبايت في buffer التي يبدأ عندها نسخ البايتات إلى التيار الحالي. |
| count | Int32 | عدد البايتات التي ستكتب إلى التيار الحالي. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | يُرمى إذا تم التخلص من التيار. |
| ArgumentNullException | *buffer* هو `null`. |

### انظر أيضًا

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


