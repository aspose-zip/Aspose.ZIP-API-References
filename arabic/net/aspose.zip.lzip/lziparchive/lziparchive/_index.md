---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP لمرجع .NET API
description: LzipArchive البناء. يقوم بتهيئة مثيل جديد لملفLzipArchive .
type: docs
weight: 10
url: /ar/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| settings | LzipArchiveSettings | إعداد أرشيف lzip خاص مع تحديد حجم القاموس. |

### أنظر أيضا

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* مساحة الاسم [Aspose.Zip.Lzip](../../lziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`LzipArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public LzipArchive(Stream sourceStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *sourceStream* لا يمكن البحث عنه. |
| ArgumentNullException | *sourceStream* باطل. |
| InvalidDataException | الرؤوس لا تتطابق مع نوع أرشيف lzip. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Extract`](../extract/) طريقة فك الضغط.

### أنظر أيضا

* class [LzipArchive](../)
* مساحة الاسم [Aspose.Zip.Lzip](../../lziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`LzipArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | الرؤوس لا تتطابق مع نوع أرشيف lzip. |

### ملاحظات

هذا المُنشئ لا يقوم بفك ضغط. يرى[`Extract`](../extract/) طريقة فك الضغط.

### أمثلة

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### أنظر أيضا

* class [LzipArchive](../)
* مساحة الاسم [Aspose.Zip.Lzip](../../lziparchive/)
* المجسم [Aspose.Zip](../../../)


