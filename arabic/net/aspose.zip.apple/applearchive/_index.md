---
title: "الفئة AppleArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "فئة Aspose.Zip.Apple.AppleArchive. تمثل هذه الفئة ملف Apple Archive بامتداد .aar. استخدمها لإنشاء ملفات Apple Archive"
type: docs
weight: 60
url: /ar/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

هذه الفئة تمثل ملف Apple Archive (.aar). استخدمها لإنشاء ملفات Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | يُهيئ مثيلًا جديدًا من الفئة `AppleArchive` باستخدام الإعدادات المستخدمة للمدخلات المُكوَّنة. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | يُهيئ مثيلًا جديدًا من الفئة `AppleArchive` ويُنشئ قائمة مدخلات يمكن استخراجها من الأرشيف. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | يُهيئ مثيلًا جديدًا من الفئة `AppleArchive` ويُنشئ قائمة مدخلات يمكن استخراجها من الأرشيف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | يحصل على المدخلات التي تُكوِّن الأرشيف. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | يحصل على قيمة تُشير إلى ما إذا كان الأرشيف يستخدم ضغطًا صلبًا. في الوضع الصلب، يتم ضغط جميع بيانات المدخلات كتيار واحد ولا يتوفر استخراج المدخلات الفردية. استخدم [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) بدلاً من ذلك. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | يحصل على الإعدادات المستخدمة للمدخلات المُكوَّنة حديثًا. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المحدد. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | ينشئ مدخلًا واحدًا داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | ينشئ مدخلًا واحدًا داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | ينشئ مدخلًا واحدًا داخل الأرشيف. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | يستخرج جميع الملفات في الأرشيف إلى الدليل المحدد. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | يحفظ الأرشيف إلى الدفق المقدم. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |

## ملاحظات

Apple و Apple Archive علامتا تجاريتان لشركة Apple Inc.

### انظر أيضًا

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


