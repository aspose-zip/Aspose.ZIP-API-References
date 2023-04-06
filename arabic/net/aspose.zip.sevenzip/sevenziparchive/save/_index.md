---
title: SevenZipArchive.Save
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchive طريقة. يحفظ أرشيف 7z في الدفق المقدم.
type: docs
weight: 80
url: /ar/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

يحفظ أرشيف 7z في الدفق المقدم.

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
| InvalidOperationException | فشل برنامج التشفير في ضغط البيانات. |

### ملاحظات

*output* يجب أن يكون قابلاً للبحث.

### أمثلة

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### أنظر أيضا

* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

لحفظ الأرشيف في ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *destinationFileName* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*destinationFileName* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*destinationFileName* مرفوض. |
| PathTooLongException | المحدد*destinationFileName*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*destinationFileName* يحتوي على نقطتين (:) في منتصف السلسلة. |

### ملاحظات

من الممكن حفظ أرشيف بنفس المسار الذي تم تحميله منه . ومع ذلك ، لا ينصح بهذا لأن هذا الأسلوب يستخدم النسخ إلى ملف مؤقت.

### أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### أنظر أيضا

* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)


