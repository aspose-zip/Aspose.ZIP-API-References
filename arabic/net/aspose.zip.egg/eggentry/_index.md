---
title: "الفئة EggEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "Aspose.Zip.Egg.EggEntry فئة. تمثل إدخال ملف في أرشيف EGG مع جميع بياناته الوصفية"
type: docs
weight: 470
url: /ar/net/aspose.zip.egg/eggentry/
---
## EggEntry class

يمثل إدخال ملف في أرشيف EGG مع جميع بياناته الوصفية.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | يحصل على الحجم المضغوط للإدخال. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان هذا الإدخال يمثل دليلًا. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | يحصل أو يعيّن تاريخ ووقت آخر تعديل. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | يحصل على اسم الإدخال داخل الأرشيف. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | يحصل على الحجم غير المضغوط للإدخال. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | يستخرج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |

### انظر أيضًا

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


