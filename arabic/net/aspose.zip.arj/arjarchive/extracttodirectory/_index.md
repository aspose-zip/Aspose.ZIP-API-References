---
title: "ArjArchive.ExtractToDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة ArjArchive. تستخرج جميع الإدخالات إلى الدليل المحدد"
type: docs
weight: 60
url: /ar/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

يستخرج جميع الإدخالات إلى الدليل المحدد.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationDirectory | String | الدليل لاستخراج الإدخالات إليه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | يتم إلقاء الاستثناء عندما يكون *destinationDirectory* فارغًا. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| NotImplementedException | الإدخال مضغوط باستخدام الطريقة 4. |

## أمثلة

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى دليل:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### انظر أيضًا

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


