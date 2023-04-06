---
title: CpioArchive.Save
second_title: Aspose.ZIP لمرجع .NET API
description: CpioArchive طريقة. لحفظ الأرشيف في ملف الوجهة المقدم.
type: docs
weight: 80
url: /ar/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

لحفظ الأرشيف في ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *destinationFileName* عبارة عن سلسلة ذات طول صفري ، أو تحتوي على مسافة بيضاء فقط ، أو تحتوي على حرف واحد غير صالح أو أكثر كما هو محدد بواسطة System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* باطل. |
| PathTooLongException | المحدد*destinationFileName*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| DirectoryNotFoundException | المحدد*destinationFileName* غير صالح (على سبيل المثال ، على محرك أقراص غير معين). |
| IOException | حدث خطأ I / O أثناء فتح الملف. |
| UnauthorizedAccessException | *destinationFileName* حدد ملفًا للقراءة فقط وكان الوصول ليس للقراءة. أو - المسار المحدد دليلًا. - أو - ليس لدى المتصل الإذن المطلوب. |
| NotSupportedException | *destinationFileName* بتنسيق غير صالح. |

### ملاحظات

من الممكن حفظ أرشيف بنفس المسار الذي تم تحميله منه . ومع ذلك ، لا ينصح بهذا لأن هذا الأسلوب يستخدم النسخ إلى ملف مؤقت.

### أمثلة

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *output* باطل. |
| ArgumentException | *output* غير قابل للكتابة. - أو -*output* هو نفس الدفق الذي نستخرج منه . - OR - من المستحيل حفظ الأرشيف في*cpioFormat* بسبب قيود التنسيق. |

### ملاحظات

*output*يجب أن يكون قابلاً للكتابة.

### أمثلة

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)


