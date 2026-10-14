---
title: "GetFormatInfo"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: 
type: docs
weight: 20
url: /ar/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

يحصل على معلومات التنسيق.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول تنسيق الأرشيف أو null إذا لم يتم اكتشاف التنسيق.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *fileName* هو null. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | *fileName* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *fileName*. |
| PathTooLongException | الـ *fileName* المحدد يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *fileName* يحتوي على نقطتين (:) في وسط السلسلة. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |

### انظر أيضًا

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

يحصل على معلومات التنسيق.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تيار | تيار | دفق ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول تنسيق الأرشيف أو null إذا لم يتم اكتشاف التنسيق.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *stream* فارغ. |
| ArgumentException | *stream* غير قابل للتمرير. |

### انظر أيضًا

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- لا تقم بالتعديل: تم الإنشاء بواسطة xmldocmd لـ Aspose.Zip.dll -->
