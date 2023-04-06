---
title: RarArchiveEntry.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: RarArchiveEntry طريقة. لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر.
type: docs
weight: 90
url: /ar/net/aspose.zip.rar/rararchiveentry/extract/
---
## Extract(string, string) {#extract}

لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر.

```csharp
public FileInfo Extract(string path, string password = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الملف الوجهة. إذا كان الملف موجودًا بالفعل ، فسيتم استبداله. |
| password | String | كلمة مرور اختيارية لفك التشفير. |

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
| InvalidDataException | فشل التحقق CRC أو MAC للإدخال. |

### أمثلة

استخراج اثنين من إدخالات أرشيف rar.

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### أنظر أيضا

* class [RarArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.Rar](../../rararchiveentry/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

لاستخراج الإدخال إلى الدفق المقدم.

```csharp
public void Extract(Stream destination, string password = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destination | Stream | تيار الوجهة. يجب أن يكون قابلاً للكتابة. |
| password | String | كلمة مرور اختيارية لفك التشفير. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidDataException | فشل التحقق CRC أو MAC للإدخال. |
| ArgumentException | *destination* لا يدعم الكتابة. |

### أمثلة

استخراج إدخال من أرشيف rar بكلمة مرور.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### أنظر أيضا

* class [RarArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.Rar](../../rararchiveentry/)
* المجسم [Aspose.Zip](../../../)


