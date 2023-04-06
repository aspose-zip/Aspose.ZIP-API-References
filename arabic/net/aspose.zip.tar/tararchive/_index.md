---
title: Class TarArchive
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Tar.TarArchive فصل. هذه الفئة تمثل ملف أرشيف tar. استخدمه لإنشاء أو استخراج أو تحديث أرشيفات tar.
type: docs
weight: 730
url: /ar/net/aspose.zip.tar/tararchive/
---
## TarArchive class

هذه الفئة تمثل ملف أرشيف tar. استخدمه لإنشاء أو استخراج أو تحديث أرشيفات tar.

```csharp
public class TarArchive : IArchive
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | يقوم بتهيئة مثيل جديد لملف`TarArchive` فئة . |
| [TarArchive](tararchive/#constructor_1)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Archive`](../../aspose.zip/archive/) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |
| [TarArchive](tararchive/#constructor_2)(string) | يقوم بتهيئة مثيل جديد لملف`TarArchive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | يحصل على إدخالات[`TarEntry`](../tarentry/) النوع الذي يشكل الأرشيف. |

## طُرق

| اسم | وصف |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | مقتطفات من أرشيف gzip وتكوينه`TarArchive` من البيانات المستخرجة. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | مقتطفات من أرشيف gzip وتكوينه`TarArchive` من البيانات المستخرجة. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | المقتطفات المقدمة أرشيف lzip ويؤلف`TarArchive` من البيانات المستخرجة. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | المقتطفات المقدمة أرشيف lzip ويؤلف`TarArchive` من البيانات المستخرجة. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | يتم توفير مقتطفات من أرشيف بتنسيق xz ويؤلف`TarArchive` من البيانات المستخرجة. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | يتم توفير مقتطفات من أرشيف بتنسيق xz ويؤلف`TarArchive` من البيانات المستخرجة. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | يتم توفير مقتطفات من أرشيف بتنسيق Z ويؤلف`TarArchive` من البيانات المستخرجة. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | يتم توفير مقتطفات من أرشيف بتنسيق Z ويؤلف`TarArchive` من البيانات المستخرجة. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | إنشاء إدخال واحد داخل الأرشيف. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | يحذف الإدخال من قائمة الإدخالات بالفهرس. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | يحفظ الأرشيف إلى الدفق المقدم. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | لحفظ الأرشيف في ملف الوجهة المقدم. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | لحفظ الأرشيف في الدفق بضغط gzip . |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | يحفظ الأرشيف إلى الملف عن طريق المسار بضغط gzip . |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | لحفظ الأرشيف في الدفق بضغط lzip . |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | يحفظ الأرشيف إلى الملف عن طريق المسار بضغط lzip . |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | يحفظ الأرشيف في الدفق بضغط xz . |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | يحفظ الأرشيف إلى المسار بالمسار بضغط xz . |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | يحفظ الأرشيف في الدفق بضغط Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | يحفظ الأرشيف إلى المسار بالمسار بضغط Z. |

### أنظر أيضا

* interface [IArchive](../../aspose.zip/iarchive/)
* مساحة الاسم [Aspose.Zip.Tar](../../aspose.zip.tar/)
* المجسم [Aspose.Zip](../../)


