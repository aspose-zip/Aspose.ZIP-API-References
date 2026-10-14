---
title: "LzxArchive.ExtractToDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة LzxArchive. تستخرج جميع الملفات والمجلدات في الأرشيف إلى الدليل المحدد"
type: docs
weight: 40
url: /ar/net/aspose.zip.lzx/lzxarchive/extracttodirectory/
---
## LzxArchive.ExtractToDirectory method

يستخرج جميع الملفات والمجلدات في الأرشيف إلى المجلد المُحدد.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationDirectory | String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *destinationDirectory* هو null. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا وأسماء الملفات أقل من 260 حرفًا. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول إلى الدليل الموجود. |
| NotSupportedException | إذا لم يكن الدليل موجودًا، فإن المسار يحتوي على حرف النقطتين (:) الذي ليس جزءًا من تسمية محرك الأقراص ("C:\"). |
| ArgumentException | *destinationDirectory* هو سلسلة بطول صفر، أو يحتوي فقط على مسافات بيضاء، أو يحتوي على حرف أو أكثر غير صالحة. يمكنك الاستعلام عن الأحرف غير الصالحة باستخدام طريقة System.IO.Path.GetInvalidPathChars. -or- المسار يبدأ بـ أو يحتوي فقط على حرف نقطتين (:). |
| IOException | الدليل المحدد بواسطة المسار هو ملف. -or- اسم الشبكة غير معروف. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidDataException | تم توفير كلمة مرور خاطئة. - أو - الأرشيف تالف. |
| NotSupportedException | طريقة ضغط غير صالحة. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |

## ملاحظات

إذا لم يكن الدليل موجودًا، سيتم إنشاؤه.

## أمثلة

```csharp
using (var archive = new LzxArchive("archive.lzx")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### انظر أيضًا

* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


