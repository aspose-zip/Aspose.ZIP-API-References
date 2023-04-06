---
title: TarArchive.ExtractToDirectory
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم.
type: docs
weight: 110
url: /ar/net/aspose.zip.tar/tararchive/extracttodirectory/
---
## TarArchive.ExtractToDirectory method

استخراج كافة الملفات الموجودة في الأرشيف إلى الدليل المقدم.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationDirectory | String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | المسار فارغ |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الطول الأقصى المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول إلى الدليل الحالي. |
| NotSupportedException | إذا لم يكن الدليل موجودًا ، فسيحتوي المسار على حرف النقطتين (:) وهو ليس جزءًا من تسمية محرك الأقراص ("C: \"). |
| ArgumentException | المسار عبارة عن سلسلة ذات طول صفري ، أو تحتوي على مسافة بيضاء فقط ، أو تحتوي على حرف أو أكثر من الأحرف غير الصالحة. يمكنك الاستعلام عن الأحرف غير الصالحة باستخدام أسلوب System.IO.Path.GetInvalidPathChars. - أو - يكون المسار مسبوقًا أو يحتوي على حرف نقطتين فقط (:). |
| IOException | الدليل المحدد بواسطة المسار هو ملف. - أو - اسم الشبكة غير معروف. |

### ملاحظات

إذا كان الدليل غير موجود ، فسيتم إنشاؤه.

### أمثلة

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


