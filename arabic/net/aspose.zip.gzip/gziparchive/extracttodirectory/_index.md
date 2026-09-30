---
title: "GzipArchive.ExtractToDirectory"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة GzipArchive. تستخرج محتوى الأرشيف إلى الدليل المقدم."
type: docs
weight: 60
url: /ar/net/aspose.zip.gzip/gziparchive/extracttodirectory/
---
## GzipArchive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* هو null. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا وأسماء الملفات أقل من 260 حرفًا. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول إلى الدليل الموجود. |
| NotSupportedException | إذا لم يكن الدليل موجودًا، يحتوي المسار على حرف نقطتين (:) ليس جزءًا من تسمية محرك الأقراص ("C:\"). |
| ArgumentException | *destinationDirectory* هو سلسلة بطول صفر، أو يحتوي فقط على مسافات بيضاء، أو يحتوي على حرف أو أكثر غير صالحة. يمكنك الاستعلام عن الأحرف غير الصالحة باستخدام طريقة System.IO.Path.GetInvalidPathChars. -or- المسار يبدأ بـ أو يحتوي فقط على حرف نقطتين (:). |
| IOException | الدليل المحدد بواسطة المسار هو ملف. -or- اسم الشبكة غير معروف. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

إذا لم يكن الدليل موجودًا، سيتم إنشاؤه.

### انظر أيضًا

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


