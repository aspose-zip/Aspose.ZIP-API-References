---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP لمرجع .NET API
description: LzmaArchive البناء. يقوم بتهيئة مثيل جديد لملفLzmaArchive فئة ويؤلف الأرشيف بتنسيق lzma.
type: docs
weight: 10
url: /ar/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`LzmaArchive`](../) فئة ويؤلف الأرشيف بتنسيق lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| settings | LzmaArchiveSettings | مجموعة من وضع أرشيف lzma معين. |

### أنظر أيضا

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* مساحة الاسم [Aspose.Zip.LZMA](../../lzmaarchive/)
* المجسم [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`LzmaArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public LzmaArchive(Stream source)
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

* class [LzmaArchive](../)
* مساحة الاسم [Aspose.Zip.LZMA](../../lzmaarchive/)
* المجسم [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`LzmaArchive`](../) فئة جاهزة لفك الضغط.

```csharp
public LzmaArchive(string path)
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
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### أنظر أيضا

* class [LzmaArchive](../)
* مساحة الاسم [Aspose.Zip.LZMA](../../lzmaarchive/)
* المجسم [Aspose.Zip](../../../)


