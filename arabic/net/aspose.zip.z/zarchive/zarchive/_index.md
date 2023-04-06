---
title: ZArchive.ZArchive
second_title: Aspose.ZIP لمرجع .NET API
description: ZArchive البناء. يقوم بتهيئة مثيل جديد لملفZArchive فئة جاهزة للضغط .
type: docs
weight: 10
url: /ar/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`ZArchive`](../) فئة جاهزة للضغط .

```csharp
public ZArchive()
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`ZArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public ZArchive(Stream source)
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

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`ZArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public ZArchive(string path)
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

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)


