---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP لمرجع .NET API
description: ParallelOptions ملكية. الحصول على تقدير الذاكرة أو تعيينه بالميغابايت المتاحة لاستيعاب الإدخالات المضغوطة دون التبديل إلى القرص . هذه القيمة تكون منطقية فقط إذاParallelCompressInMemory الإعداد فيAuto الوضع .
type: docs
weight: 20
url: /ar/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

الحصول على تقدير الذاكرة أو تعيينه بالميغابايت المتاحة لاستيعاب الإدخالات المضغوطة دون التبديل إلى القرص . هذه القيمة تكون منطقية فقط إذا[`ParallelCompressInMemory`](../parallelcompressinmemory/) الإعداد فيAuto الوضع .

```csharp
public int AvailableMemorySize { get; set; }
```

### ملاحظات

تُستخدم هذه القيمة لحساب الحجم الأكبر للإدخال الذي يمكن ضغطه بالتوازي مع الآخرين. سيتم ضغط جميع الإدخالات التي تزيد عن الحد المحسوب بالتتابع`AvailableMemorySize` ممتلكات كبيرة مثل ذاكرة الوصول العشوائي المجانية وأكبر. بشكل افتراضي ، من المفترض أن يكون لديك 200 ميجابايت على الأقل لكل نواة من وحدة المعالجة المركزية.

### أنظر أيضا

* class [ParallelOptions](../)
* مساحة الاسم [Aspose.Zip.Saving](../../paralleloptions/)
* المجسم [Aspose.Zip](../../../)


