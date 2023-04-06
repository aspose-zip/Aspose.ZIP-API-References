---
title: TarArchive.SaveGzipped
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. لحفظ الأرشيف في الدفق بضغط gzip .
type: docs
weight: 130
url: /ar/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

لحفظ الأرشيف في الدفق بضغط gzip .

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *output* باطل. |
| ArgumentException | *output* غير قابل للكتابة. |

### ملاحظات

*output*يجب أن يكون قابلاً للكتابة.

### أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

يحفظ الأرشيف إلى الملف عن طريق المسار بضغط gzip .

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |

### أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


