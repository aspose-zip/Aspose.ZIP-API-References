---
title: "LzmaArchive.ExtractToDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة LzmaArchive. تستخرج محتوى الأرشيف إلى الدليل المحدد"
type: docs
weight: 40
url: /ar/net/aspose.zip.lzma/lzmaarchive/extracttodirectory/
---
## LzmaArchive.ExtractToDirectory method

يستخرج محتوى الأرشيف إلى الدليل المقدم.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationDirectory | String | المسار إلى الدليل لوضع الملفات المستخرجة فيه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | *destinationDirectory* هو null. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا وأسماء الملفات أقل من 260 حرفًا. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول إلى الدليل الموجود. |
| NotSupportedException | إذا لم يكن الدليل موجودًا، فإن المسار يحتوي على حرف النقطتين (:) الذي ليس جزءًا من تسمية محرك الأقراص ("C:\"). |
| ArgumentException | *destinationDirectory* هو سلسلة بطول صفر، أو يحتوي فقط على مسافات بيضاء، أو يحتوي على حرف أو أكثر غير صالحة. يمكنك الاستعلام عن الأحرف غير الصالحة باستخدام طريقة System.IO.Path.GetInvalidPathChars. -or- المسار يبدأ بـ أو يحتوي فقط على حرف نقطتين (:). |
| IOException | الدليل المحدد بواسطة المسار هو ملف. -or- اسم الشبكة غير معروف. |
| InvalidDataException | الأرشيف تالف. |

## ملاحظات

إذا لم يكن الدليل موجودًا، سيتم إنشاؤه.

### انظر أيضًا

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


