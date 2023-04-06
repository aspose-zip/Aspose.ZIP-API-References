---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveInstanceInfo طريقة. يحصل على معلومات مثيل الأرشيف .
type: docs
weight: 10
url: /ar/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

يحصل على معلومات مثيل الأرشيف .

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | اسم ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول مثيل الأرشيف أو فارغة إذا لم يتم اكتشاف التنسيق.

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

* class [ArchiveInstanceInfo](../)
* مساحة الاسم [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* المجسم [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

يحصل على معلومات مثيل الأرشيف .

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار ملف الأرشيف. |

### قيمة الإرجاع

معلومات حول مثيل الأرشيف أو فارغة إذا لم يتم اكتشاف التنسيق.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *stream* باطل. |
| ArgumentException | *stream* لا يمكن البحث عنه. |

### أنظر أيضا

* class [ArchiveInstanceInfo](../)
* مساحة الاسم [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* المجسم [Aspose.Zip](../../../)


