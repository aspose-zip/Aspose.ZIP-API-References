---
title: Class CpioArchive
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Cpio.CpioArchive فصل. تمثل هذه الفئة ملف أرشيف cpio .
type: docs
weight: 160
url: /ar/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

تمثل هذه الفئة ملف أرشيف cpio .

```csharp
public class CpioArchive : IArchive
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | يقوم بتهيئة مثيل جديد لملف`CpioArchive` فئة . |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | يقوم بتهيئة مثيل جديد لملف`CpioArchive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | يقوم بتهيئة مثيل جديد لملف`CpioArchive` يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | يحصل على إدخالات[`CpioEntry`](../cpioentry/) النوع الذي يشكل الأرشيف. |

## طُرق

| اسم | وصف |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | إنشاء إدخال واحد داخل الأرشيف. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | إنشاء إدخال واحد داخل الأرشيف. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | يحذف الإدخال من قائمة الإدخالات بالفهرس. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | يحفظ الأرشيف إلى الدفق المقدم. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | لحفظ الأرشيف في ملف الوجهة المقدم. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | لحفظ الأرشيف في الدفق بضغط gzip . |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | يحفظ الأرشيف إلى الملف عن طريق المسار بضغط gzip . |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | يحفظ الأرشيف في الدفق بضغط xz . |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | يحفظ الأرشيف إلى المسار بالمسار بضغط xz . |

### أنظر أيضا

* interface [IArchive](../../aspose.zip/iarchive/)
* مساحة الاسم [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* المجسم [Aspose.Zip](../../)


