---
title: Class XarFileEntry
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Xar.XarFileEntry فصل. يمثل إدخال الملف داخل أرشيف xar .
type: docs
weight: 840
url: /ar/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

يمثل إدخال الملف داخل أرشيف xar .

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | يحصل على وقت إنشاء الملف أو الدليل. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | يحصل على المسار الكامل للإدخال داخل الأرشيف. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الإدخال يمثل الدليل . |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | يحصل على آخر وقت وصول للملف أو الدليل. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | يحصل على وقت تعديل الملف أو الدليل. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | الحصول على طول الإدخال بالبايت. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | الحصول على اسم الإدخال داخل الأرشيف. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | الحصول على الدليل الأصلي الذي ينتمي إليه الإدخال . |

## طُرق

| اسم | وصف |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | لاستخراج الإدخال إلى الدفق المقدم. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | يفتح الإدخال للاستخراج ويوفر دفقًا بمحتوى الإدخال. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### أنظر أيضا

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* مساحة الاسم [Aspose.Zip.Xar](../../aspose.zip.xar/)
* المجسم [Aspose.Zip](../../)


