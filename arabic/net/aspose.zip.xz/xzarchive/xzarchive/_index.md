---
title: XzArchive.XzArchive
second_title: Aspose.ZIP لمرجع .NET API
description: XzArchive البناء. يقوم بتهيئة مثيل جديد لملفXzArchive class ويؤلف الأرشيف بتنسيق xz.
type: docs
weight: 10
url: /ar/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`XzArchive`](../) class ويؤلف الأرشيف بتنسيق xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| settings | XzArchiveSettings | مجموعة من الإعدادات الخاصة بأرشيف xz: حجم القاموس ، حجم الكتلة ، نوع الاختيار. |

### أنظر أيضا

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`XzArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public XzArchive(Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Stream | مصدر الأرشيف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *source* لا يمكن البحث عنه. |
| ArgumentNullException | *source* باطل. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Extract`](../extract/) طريقة فك الضغط.

### أنظر أيضا

* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`XzArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public XzArchive(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | الطريق إلى مصدر الأرشيف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Extract`](../extract/) طريقة فك الضغط.

### أنظر أيضا

* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)


