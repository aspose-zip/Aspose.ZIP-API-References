---
title: Class ArchiveEntry
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.ArchiveEntry فصل. يمثل ملفًا واحدًا داخل الأرشيف.
type: docs
weight: 20
url: /ar/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

يمثل ملفًا واحدًا داخل الأرشيف.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
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
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | لاستخراج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى إدخال غير مضغوط. |

## الأحداث

| اسم | وصف |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | يتم رفعه عند ضغط جزء من التدفق الخام. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | يتم رفعه عند استخراج جزء من الدفق الخام. |

### ملاحظات

يلقي و`ArchiveEntry` مثال ل[`ArchiveEntryEncrypted`](../archiveentryencrypted/) لتحديد ما إذا كان الإدخال مشفرًا أم لا.

### أنظر أيضا

* interface [IArchiveFileEntry](../iarchivefileentry/)
* مساحة الاسم [Aspose.Zip](../../aspose.zip/)
* المجسم [Aspose.Zip](../../)


