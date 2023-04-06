---
title: Class RarArchiveEntry
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Rar.RarArchiveEntry فصل. يمثل ملفًا واحدًا داخل الأرشيف.
type: docs
weight: 320
url: /ar/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

يمثل ملفًا واحدًا داخل الأرشيف.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | يحصل على حجم الملف المضغوط. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | يحصل على تاريخ ووقت الإنشاء . |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل الدليل . |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | الحصول على تاريخ ووقت آخر وصول. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | الحصول على تاريخ ووقت آخر تعديل. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | الحصول على اسم الإدخال داخل الأرشيف. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | يحصل على حجم الملف الأصلي. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | لاستخراج الإدخال إلى الدفق المقدم. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى إدخال غير مضغوط. |

## الأحداث

| اسم | وصف |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | يتم رفعه عند استخراج جزء من الدفق الخام. |

### ملاحظات

يلقي أ`RarArchiveEntry` مثال ل[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) لتحديد ما إذا كان الإدخال مشفرًا أم لا.

### أنظر أيضا

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* مساحة الاسم [Aspose.Zip.Rar](../../aspose.zip.rar/)
* المجسم [Aspose.Zip](../../)


