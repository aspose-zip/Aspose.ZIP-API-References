---
title: TarArchive.FromGZip
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. مقتطفات من أرشيف gzip وتكوينهTarArchive من البيانات المستخرجة.
type: docs
weight: 20
url: /ar/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

مقتطفات من أرشيف gzip وتكوينه[`TarArchive`](../) من البيانات المستخرجة.

هام: يتم استخراج أرشيف gzip بالكامل ضمن هذه الطريقة ، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromGZip(Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Stream | مصدر الأرشيف. |

### قيمة الإرجاع

مثال على[`TarArchive`](../)

### ملاحظات

لا يمكن البحث عن تيار استخراج GZip من خلال طبيعة خوارزمية الضغط. يوفر أرشيف Tar وسيلة لاستخراج السجل التعسفي ، لذلك يتعين عليه تشغيل تيار يمكن البحث عنه تحت الغطاء.

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

مقتطفات من أرشيف gzip وتكوينه[`TarArchive`](../) من البيانات المستخرجة.

هام: يتم استخراج أرشيف gzip بالكامل ضمن هذه الطريقة ، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromGZip(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار إلى ملف الأرشيف. |

### قيمة الإرجاع

مثال على[`TarArchive`](../)

### ملاحظات

لا يمكن البحث عن تيار استخراج GZip من خلال طبيعة خوارزمية الضغط. يوفر أرشيف Tar وسيلة لاستخراج السجل التعسفي ، لذلك يتعين عليه تشغيل تيار يمكن البحث عنه تحت الغطاء.

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


