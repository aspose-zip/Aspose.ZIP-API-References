---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchiveEntry طريقة. لاستخراج الإدخال إلى نظام الملفات من خلال المسار المتوفر.
type: docs
weight: 80
url: /ar/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
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

### أمثلة

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
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
| ArgumentException | *destination* لا يدعم الكتابة. |
| InvalidOperationException | الأرشيف غير مفتوح للاستخراج. - أو - هذا الإدخال هو دليل. |
| InvalidDataException | بيانات خاطئة داخل الإدخال. |

### أمثلة

استخراج إدخال من أرشيف مضغوط بكلمة مرور.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* المجسم [Aspose.Zip](../../../)


