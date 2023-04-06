---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP لمرجع .NET API
description: CpioArchive طريقة. يحفظ الأرشيف في الدفق بضغط xz .
type: docs
weight: 100
url: /ar/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

يحفظ الأرشيف في الدفق بضغط xz .

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |
| settings | XzArchiveSettings | مجموعة من الإعدادات الخاصة بأرشيف xz: حجم القاموس ، حجم الكتلة ، نوع الاختيار. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *output* باطل. |
| ArgumentException | *output* غير قابل للكتابة. |

### ملاحظات

*output*يجب أن يكون الدفق قابلاً للكتابة.

### أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

يحفظ الأرشيف إلى المسار بالمسار بضغط xz .

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |
| settings | XzArchiveSettings | مجموعة من الإعدادات الخاصة بأرشيف xz: حجم القاموس ، حجم الكتلة ، نوع الاختيار. |

### أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)


