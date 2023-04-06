---
title: Class ParallelOptions
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Saving.ParallelOptions فصل. خيارات للضغط المتوازي .
type: docs
weight: 490
url: /ar/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

خيارات للضغط المتوازي .

```csharp
public class ParallelOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | الحصول على تقدير الذاكرة أو تعيينه بالميغابايت المتاحة لاستيعاب الإدخالات المضغوطة دون التبديل إلى القرص . هذه القيمة تكون منطقية فقط إذا[`ParallelCompressInMemory`](./parallelcompressinmemory/) الإعداد فيAuto الوضع . |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى كيفية استخدام النهج المتوازي. |

### ملاحظات

تدير هذه الخيارات الضغط المتزامن بواسطة عدة مراكز CPU.

### أمثلة

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### أنظر أيضا

* مساحة الاسم [Aspose.Zip.Saving](../../aspose.zip.saving/)
* المجسم [Aspose.Zip](../../)


