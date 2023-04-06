---
title: Class GzipArchive
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Gzip.GzipArchive فصل. تمثل هذه الفئة ملف أرشيف gzip. استخدمه لإنشاء أو استخراج أرشيفات gzip.
type: docs
weight: 210
url: /ar/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

تمثل هذه الفئة ملف أرشيف gzip. استخدمه لإنشاء أو استخراج أرشيفات gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | يقوم بتهيئة مثيل جديد لملف`GzipArchive` فئة جاهزة للضغط . |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | يقوم بتهيئة مثيل جديد لملف`GzipArchive` فئة جاهزة لفك الضغط. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | يقوم بتهيئة مثيل جديد لملف`GzipArchive` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | اسم الملف الأصلي . |

## طُرق

| اسم | وصف |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | لاستخراج الأرشيف إلى الدفق المقدم. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | يفتح الأرشيف للاستخراج ويوفر دفقًا بمحتوى أرشيف. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | يحفظ الأرشيف إلى الدفق المقدم. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | لحفظ الأرشيف في ملف الوجهة المقدم. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | يحدد المحتوى المراد ضغطه داخل الأرشيف. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | يحدد المحتوى المراد ضغطه داخل الأرشيف. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | يحدد المحتوى المراد ضغطه داخل الأرشيف. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | يحدد المحتوى المراد ضغطه داخل الأرشيف. |

### ملاحظات

تعتمد خوارزمية ضغط Gzip على خوارزمية DEFLATE ، وهي مزيج من ترميز LZ77 و Huffman.

### أنظر أيضا

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* مساحة الاسم [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* المجسم [Aspose.Zip](../../)


