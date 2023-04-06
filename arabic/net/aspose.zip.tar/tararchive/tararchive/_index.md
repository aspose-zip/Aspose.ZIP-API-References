---
title: TarArchive.TarArchive
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive البناء. يقوم بتهيئة مثيل جديد لملفTarArchive فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`TarArchive`](../) فئة .

```csharp
public TarArchive()
```

### أمثلة

يوضح المثال التالي كيفية ضغط ملف.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Archive`](../../../aspose.zip/archive/) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public TarArchive(Stream sourceStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. يجب أن يكون قابلاً للبحث. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidDataException | *sourceStream* لا يمكن البحث عنه. |

### ملاحظات

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../tarentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`TarArchive`](../) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public TarArchive(string path)
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

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. يرى[`Open`](../../tarentry/open/)طريقة التفريغ .

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الإدخالات إلى دليل.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


