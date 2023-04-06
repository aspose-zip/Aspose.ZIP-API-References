---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. يحفظ الأرشيف في الدفق بضغط xz .
type: docs
weight: 150
url: /ar/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

يحفظ الأرشيف في الدفق بضغط xz .

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |
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
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

يحفظ الأرشيف إلى المسار بالمسار بضغط xz .

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |
| format | Nullable`1 | يحدد تنسيق رأس القطران. سيتم التعامل مع القيمة الفارغة على أنها USTar عندما يكون ذلك ممكنًا. |
| settings | XzArchiveSettings | مجموعة من الإعدادات الخاصة بأرشيف xz: حجم القاموس ، حجم الكتلة ، نوع الاختيار. |

### أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### أنظر أيضا

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


