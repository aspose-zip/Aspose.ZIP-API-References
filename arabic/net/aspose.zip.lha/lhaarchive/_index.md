---
title: "الفئة LhaArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "الفئة Aspose.Zip.Lha.LhaArchive. تمثل هذه الفئة ملف أرشيف LHA .lzh"
type: docs
weight: 630
url: /ar/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

هذه الفئة تمثل ملف أرشيف LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | يُنشئ مثيلاً جديداً للفئة `LhaArchive` ويُكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | يُنشئ مثيلاً جديداً للفئة `LhaArchive` ويُكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | يحصل على مدخلات الملفات من النوع [`LhaArchiveEntry`](../lhaarchiveentry/) التي تُكوّن الأرشيف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | يستخرج جميع الملفات والمجلدات في الأرشيف إلى المجلد المُحدد. |

## ملاحظات

الطرق التالية فقط للضغط مدعومة:

**Method**

**Explanation**

**lh0**

غير مضغوط

**lh4**

قاموس انزلاقي بحجم 8 كيبايت وHuffman ثابت

**lh5**

قاموس انزلاقي بحجم 16 كيبايت وHuffman ثابت

**lh6**

قاموس انزلاقي بحجم 64 كيبايت وHuffman ثابت

**lh7**

قاموس انزلاقي بحجم 128 كيبايت وHuffman ثابت

**lhx**

قاموس انزلاقي بحجم 1 ميبيبايت وHuffman ثابت

**lhd**

مجلد

### انظر أيضًا

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


