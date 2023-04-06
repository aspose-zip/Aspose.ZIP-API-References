---
title: CpioArchive.SaveGzipped
second_title: Aspose.ZIP لمرجع .NET API
description: CpioArchive طريقة. لحفظ الأرشيف في الدفق بضغط gzip .
type: docs
weight: 90
url: /ar/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

لحفظ الأرشيف في الدفق بضغط gzip .

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *output* باطل. |
| ArgumentException | *output* غير قابل للكتابة. |

### ملاحظات

*output*يجب أن يكون قابلاً للكتابة.

### أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

يحفظ الأرشيف إلى الملف عن طريق المسار بضغط gzip .

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### أنظر أيضا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)


