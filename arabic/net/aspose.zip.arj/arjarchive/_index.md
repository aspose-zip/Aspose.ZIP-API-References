---
title: "الفئة ArjArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "الفئة Aspose.Zip.Arj.ArjArchive. تمثل هذه الفئة ملف أرشيف ARJ"
type: docs
weight: 250
url: /ar/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

هذه الفئة تمثل ملف أرشيف ARJ.

```csharp
public class ArjArchive : IArchive
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | ينشئ مثيلًا جديدًا للفئة `ArjArchive` ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | ينشئ مثيلًا جديدًا للفئة `ArjArchive` ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | يحصل على التعليق. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | يحصل على الإدخالات من النوع [`ArjEntryPlain`](../arjentryplain/) التي تشكل أرشيف ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | يحصل على الاسم الأصلي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | يستخرج جميع الإدخالات إلى الدليل المحدد. |

## ملاحظات

الطرق التالية فقط للضغط مدعومة:

**Method**

**Explanation**

**0**

غير مضغوط

**1**

مزيج من LZ77 وترميز هوفمان التكيفي. أفضل نسبة.

**2**

مزيج من LZ77 وترميز هوفمان التكيفي.

**3**

مزيج من LZ77 وترميز هوفمان التكيفي. أفضل سرعة.

### انظر أيضًا

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


