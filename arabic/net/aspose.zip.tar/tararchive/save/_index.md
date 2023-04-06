---
title: TarArchive.Save
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. يحفظ الأرشيف إلى الدفق المقدم.
type: docs
weight: 120
url: /ar/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *output* غير قابل للكتابة. - أو -*output* هو نفس الدفق الذي نستخرج منه . - OR - من المستحيل حفظ الأرشيف في*format* بسبب قيود التنسيق. |

### ملاحظات

*output*يجب أن يكون قابلاً للكتابة.

### أمثلة

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

لحفظ الأرشيف في ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |

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
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


