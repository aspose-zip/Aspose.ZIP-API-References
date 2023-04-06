---
title: ZArchive.Save
second_title: Aspose.ZIP لمرجع .NET API
description: ZArchive طريقة. يحفظ أرشيف xz في الدفق المقدم.
type: docs
weight: 40
url: /ar/net/aspose.zip.z/zarchive/save/
---
## Save(Stream) {#save}

يحفظ أرشيف xz في الدفق المقدم.

```csharp
public void Save(Stream output)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *output* لا يدعم السعي. |
| ArgumentNullException | *output* باطل. |

### ملاحظات

*output* يجب أن يكون قابلاً للبحث.

### أمثلة

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

يحفظ أرشيف Z إلى ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationFileName | String | + مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *destinationFileName* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*destinationFileName* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*destinationFileName* مرفوض. |
| PathTooLongException | المحدد*destinationFileName*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*destinationFileName* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)


