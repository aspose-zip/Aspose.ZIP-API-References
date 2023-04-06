---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry فصل. يمثل ملفًا واحدًا داخل أرشيف 7z .
type: docs
weight: 670
url: /ar/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

يمثل ملفًا واحدًا داخل أرشيف 7z .

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | يحصل على حجم الملف المضغوط. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | الحصول على إعدادات للضغط أو فك الضغط . |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل الدليل . |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | الحصول على تاريخ ووقت آخر تعديل. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | الحصول على اسم الإدخال داخل الأرشيف. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | يحصل على حجم الملف الأصلي. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | لاستخراج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال. |

## الأحداث

| اسم | وصف |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | يتم رفعه عند ضغط جزء من التدفق الخام. |

### ملاحظات

يلقي و`SevenZipArchiveEntry` مثال ل[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) لتحديد ما إذا كان الإدخال مشفرًا أم لا.

### أنظر أيضا

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* مساحة الاسم [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* المجسم [Aspose.Zip](../../)


