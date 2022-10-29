---
title: Bzip2CompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: يقوم بتهيئة مثيل جديد لملفBzip2CompressionSettingsaspose.zip.saving/bzip2compressionsettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Bzip2CompressionSettings`](../../bzip2compressionsettings) فئة .

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

* class [Bzip2CompressionSettings](../../bzip2compressionsettings)
* مساحة الاسم [Aspose.Zip.Saving](../../bzip2compressionsettings)
* المجسم [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Bzip2CompressionSettings`](../../bzip2compressionsettings)فئة بحجم الكتلة الافتراضي ، تساوي 9 مائة كيلو بايت.

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

* class [Bzip2CompressionSettings](../../bzip2compressionsettings)
* مساحة الاسم [Aspose.Zip.Saving](../../bzip2compressionsettings)
* المجسم [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->