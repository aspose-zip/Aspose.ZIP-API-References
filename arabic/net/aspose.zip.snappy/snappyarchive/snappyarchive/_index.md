---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP لمرجع .NET API
description: SnappyArchive البناء. يقوم بتهيئة مثيل جديد لملفSnappyArchive فئة جاهزة للضغط .
type: docs
weight: 10
url: /ar/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`SnappyArchive`](../) فئة جاهزة للضغط .

```csharp
public SnappyArchive()
```

### أمثلة

يوضح المثال التالي كيفية ضغط ملف.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`SnappyArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`SnappyArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public SnappyArchive(string path)
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

### أمثلة

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)


