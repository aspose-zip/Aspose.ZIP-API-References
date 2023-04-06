---
title: WimArchive.WimArchive
second_title: Aspose.ZIP لمرجع .NET API
description: WimArchive البناء. يقوم بتهيئة مثيل جديد لملفWimArchive يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.
type: docs
weight: 10
url: /ar/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`WimArchive`](../) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public WimArchive(Stream sourceStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. يجب أن يكون قابلاً للبحث. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *sourceStream* باطل. |
| ArgumentException | *sourceStream* لا يمكن البحث عنه. |
| InvalidDataException | *sourceStream* ليس أرشيف wim صالحًا. |

### ملاحظات

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../wimfileentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### أنظر أيضا

* class [WimArchive](../)
* مساحة الاسم [Aspose.Zip.Wim](../../wimarchive/)
* المجسم [Aspose.Zip](../../../)

---

## WimArchive(string) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`WimArchive`](../) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public WimArchive(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار إلى ملف الأرشيف. |

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

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../wimfileentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### أنظر أيضا

* class [WimArchive](../)
* مساحة الاسم [Aspose.Zip.Wim](../../wimarchive/)
* المجسم [Aspose.Zip](../../../)


