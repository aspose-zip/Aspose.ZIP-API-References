---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2Archive البناء. يقوم بتهيئة مثيل جديد لملفBzip2Archive فئة جاهزة للضغط .
type: docs
weight: 10
url: /ar/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Bzip2Archive`](../) فئة جاهزة للضغط .

```csharp
public Bzip2Archive()
```

### أمثلة

يوضح المثال التالي كيفية ضغط ملف.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Bzip2Archive`](../) فئة جاهزة لفك الضغط.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Open`](../open/) طريقة فك الضغط.

### أمثلة

افتح أرشيفًا من دفق واستخرجه إلى ملف`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`Bzip2Archive`](../) فئة جاهزة لفك الضغط.

```csharp
public Bzip2Archive(string path)
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

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Open`](../open/) طريقة فك الضغط.

### أمثلة

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى ملف`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)


