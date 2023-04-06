---
title: WimFileEntry.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: WimFileEntry طريقة. لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر.
type: docs
weight: 20
url: /ar/net/aspose.zip.wim/wimfileentry/extract/
---
## Extract(string) {#extract}

لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر.

```csharp
public FileInfo Extract(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الملف الوجهة. إذا كان الملف موجودًا بالفعل ، فسيتم استبداله. |

### قيمة الإرجاع

معلومات الملف المكونة للملف.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract("data.bin");
}
```

### أنظر أيضا

* class [WimFileEntry](../)
* مساحة الاسم [Aspose.Zip.Wim](../../wimfileentry/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

لاستخراج الإدخال إلى الدفق المقدم.

```csharp
public void Extract(Stream destination)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destination | Stream | تيار الوجهة. يجب أن يكون قابلاً للكتابة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *destination* لا يدعم الكتابة. |

### أمثلة

استخراج إدخال من أرشيف ويم.

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract(httpResponseStream);
}
```

### أنظر أيضا

* class [WimFileEntry](../)
* مساحة الاسم [Aspose.Zip.Wim](../../wimfileentry/)
* المجسم [Aspose.Zip](../../../)


