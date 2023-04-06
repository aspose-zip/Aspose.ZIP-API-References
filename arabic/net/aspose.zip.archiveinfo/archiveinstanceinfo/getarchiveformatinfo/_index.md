---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveInstanceInfo طريقة. يحصل على معلومات تنسيق الأرشيف .
type: docs
weight: 50
url: /ar/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

يحصل على معلومات تنسيق الأرشيف .

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | اسم ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول تنسيق الأرشيف أو فارغة إذا لم يتم اكتشاف التنسيق.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *fileName* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*fileName* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*fileName* مرفوض. |
| PathTooLongException | المحدد*fileName* يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*fileName* يحتوي على نقطتين (:) في منتصف السلسلة. |
| IOException | حدث خطأ I / O أثناء فتح الملف. |

### أنظر أيضا

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* مساحة الاسم [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* المجسم [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

يحصل على معلومات تنسيق الأرشيف .

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول تنسيق الأرشيف أو فارغة إذا لم يتم اكتشاف التنسيق.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *stream* باطل. |
| ArgumentException | *stream* لا يمكن البحث عنه. |

### أنظر أيضا

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* مساحة الاسم [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* المجسم [Aspose.Zip](../../../)


