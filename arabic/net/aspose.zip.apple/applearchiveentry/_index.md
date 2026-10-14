---
title: "الفئة AppleArchiveEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "فئة Aspose.Zip.Apple.AppleArchiveEntry. تمثل إدخال نظام ملفات داخل AppleArchive"
type: docs
weight: 70
url: /ar/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

تمثل إدخال نظام ملفات داخل [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل دليلًا. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل ارتباطًا رمزيًا. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | يحصل على الطول غير المضغوط للإدخال بالبايت. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | يحصل على مسار الإدخال داخل الأرشيف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | يستخرج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | يفتح الإدخال للاستخراج ويوفر تدفقًا بمحتوى الإدخال. |

## ملاحظات

يمكن لنسخة من هذه الفئة تمثيل ملف عادي أو دليل أو ارتباط رمزي تم تحليله من أرشيف Apple موجود، أو ملف أو دليل تمت إضافته إلى أرشيف قيد الإنشاء.

### انظر أيضًا

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


