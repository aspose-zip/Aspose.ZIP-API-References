---
title: Class Archive
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Archive فصل. هذه الفئة تمثل ملف أرشيف مضغوط. استخدمه لإنشاء أو استخراج أو تحديث أرشيفات مضغوطة.
type: docs
weight: 10
url: /ar/net/aspose.zip/archive/
---
## Archive class

هذه الفئة تمثل ملف أرشيف مضغوط. استخدمه لإنشاء أو استخراج أو تحديث أرشيفات مضغوطة.

```csharp
public class Archive : IArchive
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | يقوم بتهيئة مثيل جديد لملف`Archive` فئة مع إعدادات اختيارية لإدخالاتها. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | يقوم بتهيئة مثيل جديد لملف`Archive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | يقوم بتهيئة مثيل جديد لملف`Archive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | يحصل على إدخالات[`ArchiveEntry`](../archiveentry/) النوع الذي يشكل الأرشيف. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | إعدادات الضغط والتشفير المستخدمة حديثًا[`ArchiveEntry`](../archiveentry/) العناصر . |

## طُرق

| اسم | وصف |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | إنشاء إدخال واحد داخل الأرشيف. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | يحذف الإدخال من قائمة الإدخالات بالفهرس. |
| [Dispose](../../aspose.zip/archive/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | يحفظ الأرشيف إلى الدفق المقدم. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | لحفظ الأرشيف في ملف الوجهة المقدم. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم. |

### أنظر أيضا

* interface [IArchive](../iarchive/)
* مساحة الاسم [Aspose.Zip](../../aspose.zip/)
* المجسم [Aspose.Zip](../../)


