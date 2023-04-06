---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2CompressionSettings البناء. يقوم بتهيئة مثيل جديد لملفBzip2CompressionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Bzip2CompressionSettings`](../) فئة .

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| blockSize | Int32 | حجم الكتلة بمئات الكيلو بايت. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | حجم الكتلة لا يتراوح بين 1 و 9. |

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [Bzip2CompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Bzip2CompressionSettings`](../) فئة بحجم الكتلة الافتراضي ، تساوي 9 مائة كيلو بايت.

```csharp
public Bzip2CompressionSettings()
```

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [Bzip2CompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* المجسم [Aspose.Zip](../../../)


