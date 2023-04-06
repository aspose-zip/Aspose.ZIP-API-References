---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP لمرجع .NET API
description: GzipArchive البناء. يقوم بتهيئة مثيل جديد لملفGzipArchive فئة جاهزة للضغط .
type: docs
weight: 10
url: /ar/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`GzipArchive`](../) فئة جاهزة للضغط .

```csharp
public GzipArchive()
```

### أمثلة

يوضح المثال التالي كيفية ضغط ملف.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`GzipArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. |
| parseHeader | Boolean | ما إذا كان سيتم تحليل رأس الدفق لمعرفة الخصائص ، بما في ذلك الاسم. من المنطقي لتيار يمكن البحث عنه فقط. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Open`](../open/) طريقة فك الضغط.

### أمثلة

افتح أرشيفًا من دفق واستخرجه إلى ملف`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`GzipArchive`](../) فئة .

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار إلى ملف الأرشيف. |
| parseHeader | Boolean | ما إذا كان سيتم تحليل رأس الدفق لمعرفة الخصائص ، بما في ذلك الاسم. من المنطقي لتيار يمكن البحث عنه فقط. |

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
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)


