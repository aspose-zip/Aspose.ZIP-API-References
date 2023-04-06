---
title: Class SevenZipArchive
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.SevenZip.SevenZipArchive فصل. هذه الفئة تمثل ملف أرشيف 7z. استخدمه لتأليف واستخراج أرشيفات 7z.
type: docs
weight: 660
url: /ar/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

هذه الفئة تمثل ملف أرشيف 7z. استخدمه لتأليف واستخراج أرشيفات 7z.

```csharp
public class SevenZipArchive : IArchive
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | يقوم بتهيئة مثيل جديد لملف`SevenZipArchive` فئة مع إعدادات اختيارية لإدخالاتها. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | يقوم بتهيئة مثيل جديد لملف`SevenZipArchive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | يقوم بتهيئة مثيل جديد لملف`SevenZipArchive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | يحصل على إدخالات[`SevenZipArchiveEntry`](../sevenziparchiveentry/) النوع الذي يشكل الأرشيف. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | إعدادات الضغط والتشفير المستخدمة حديثًا[`SevenZipArchiveEntry`](../sevenziparchiveentry/) العناصر . |

## طُرق

| اسم | وصف |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | يحفظ أرشيف 7z في الدفق المقدم. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | لحفظ الأرشيف في ملف الوجهة المقدم. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم. |

### أنظر أيضا

* interface [IArchive](../../aspose.zip/iarchive/)
* مساحة الاسم [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* المجسم [Aspose.Zip](../../)


