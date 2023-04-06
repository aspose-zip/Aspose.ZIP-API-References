---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2SaveOptions البناء. يقوم بتهيئة مثيل جديد لملفBzip2SaveOptions فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Bzip2SaveOptions`](../) فئة .

```csharp
public Bzip2SaveOptions(int blockSize)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| blockSize | Int32 | حجم الكتلة بمئات الكيلو بايت. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | حجم الكتلة ليس في النطاق الصالح. |

### أمثلة

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### أنظر أيضا

* class [Bzip2SaveOptions](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* المجسم [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Bzip2SaveOptions`](../) فئة بحجم الكتلة الافتراضي ، تساوي 9 مائة كيلو بايت.

```csharp
public Bzip2SaveOptions()
```

### أمثلة

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### أنظر أيضا

* class [Bzip2SaveOptions](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* المجسم [Aspose.Zip](../../../)


