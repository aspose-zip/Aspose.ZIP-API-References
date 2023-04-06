---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP لمرجع .NET API
description: CpioArchive البناء. يقوم بتهيئة مثيل جديد لملفCpioArchive فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`CpioArchive`](../) فئة .

```csharp
public CpioArchive()
```

### أمثلة

يوضح المثال التالي كيفية ضغط ملف.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### أنظر أيضا

* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`CpioArchive`](../) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public CpioArchive(Stream sourceStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. يجب أن يكون قابلاً للبحث. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *sourceStream* باطل. |
| ArgumentException | *sourceStream* لا يمكن البحث عنه. |
| InvalidDataException | *sourceStream* ليس أرشيف cpio صالحًا. |

### ملاحظات

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../cpioentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### أنظر أيضا

* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`CpioArchive`](../) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public CpioArchive(string path)
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

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../cpioentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### أنظر أيضا

* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)


