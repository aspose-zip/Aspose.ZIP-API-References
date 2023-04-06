---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.ArchiveEntryEncrypted فصل. إدخال مضغوط يحتاج إلى ضغطه بالتشفير أو فك ضغطه باستخدام فك التشفير .
type: docs
weight: 30
url: /ar/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

إدخال مضغوط يحتاج إلى ضغطه بالتشفير أو فك ضغطه باستخدام فك التشفير .

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | الحصول على تعليق على الإدخال داخل الأرشيف. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | يحصل على حجم الملف المضغوط. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | الحصول على إعدادات للضغط أو فك الضغط . |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | الحصول على إعدادات التشفير أو فك التشفير. |
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


