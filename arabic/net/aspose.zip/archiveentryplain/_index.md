---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.ArchiveEntryPlain فصل. إدخال مضغوط يحتاج إلى ضغطه بدون تشفير أو فك ضغطه بدون فك تشفير.
type: docs
weight: 40
url: /ar/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

إدخال مضغوط يحتاج إلى ضغطه بدون تشفير أو فك ضغطه بدون فك تشفير.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | الحصول على تعليق على الإدخال داخل الأرشيف. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | يحصل على حجم الملف المضغوط. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | الحصول على إعدادات للضغط أو فك الضغط . |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل الدليل . |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | الحصول على أو تعيين تاريخ ووقت آخر تعديل. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | الحصول على اسم الإدخال داخل الأرشيف. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | يحصل على حجم الملف الأصلي. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | لاستخراج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى إدخال غير مضغوط. |

## الأحداث

| اسم | وصف |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | يتم رفعه عند ضغط جزء من التدفق الخام. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | يتم رفعه عند استخراج جزء من الدفق الخام. |

### أنظر أيضا

* class [ArchiveEntry](../archiveentry/)
* مساحة الاسم [Aspose.Zip](../../aspose.zip/)
* المجسم [Aspose.Zip](../../)


