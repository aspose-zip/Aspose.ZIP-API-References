---
title: "الفئة AlzEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "فئة Aspose.Zip.Alz.AlzEntry. تمثل إدخال ملف في أرشيف ALZ مع جميع بياناته الوصفية."
type: docs
weight: 30
url: /ar/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

يمثل إدخال ملف في أرشيف ALZ مع جميع بياناته الوصفية.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | الحجم المضغوط لبيانات الملف بالبايت. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | يعيد true إذا كان هذا الإدخال يمثل دليلًا. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | اسم الملف (بدون المسار). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | الحجم غير المضغوط لبيانات الملف بالبايت. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | يستخرج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال غير المضغوط. |

### انظر أيضًا

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


