---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ XarBzip2CompressionSettings. يهيئ مثيلاً جديداً من الفئة XarBzip2CompressionSettings"
type: docs
weight: 10
url: /ar/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

يهيئ مثيلاً جديداً من الفئة [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | Int32 | حجم الكتلة بالمئات من الكيلوبايت. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentOutOfRangeException | حجم الكتلة ليس بين 1 و 9. |

## أمثلة

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### انظر أيضًا

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

يهيئ مثيلاً جديداً من الفئة [`XarBzip2CompressionSettings`](../) بحجم كتلة افتراضي يساوي 9 مئات من الكيلوبايت.

```csharp
public XarBzip2CompressionSettings()
```

### انظر أيضًا

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


