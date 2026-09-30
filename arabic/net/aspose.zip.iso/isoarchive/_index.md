---
title: "الفئة IsoArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "Aspose.Zip.Iso.IsoArchive فئة. يمثل أرشيف ISO ISO 9660"
type: docs
weight: 570
url: /ar/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

يمثل أرشيف ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | يُنشئ مثيلاً جديدًا من فئة `IsoArchive` ويُنشئ أرشيف ISO فارغًا لإضافة ملفات وأدلة جديدة. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | يُنشئ مثيلاً جديدًا من فئة `IsoArchive` ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | يُنشئ مثيلاً جديدًا من فئة `IsoArchive` ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | يحصل على الإدخالات من نوع [`IsoEntry`](../isoentry/) التي تُكوّن الأرشيف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | يضيف دليلًا إلى صورة ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | يضيف ملفًا إلى صورة ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | يضيف ملفًا إلى صورة ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | يضيف ملفًا إلى صورة ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | يستخرج جميع الإدخالات إلى الدليل المحدد. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | يحفظ صورة ISO إلى الدفق المحدد. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | يحفظ صورة ISO إلى المسار المحدد. |

### انظر أيضًا

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


