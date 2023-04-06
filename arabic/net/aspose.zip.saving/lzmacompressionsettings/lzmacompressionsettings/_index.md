---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: LzmaCompressionSettings البناء. يقوم بتهيئة مثيل جديد لملفLzmaCompressionSettingsفئة بحجم القاموس الافتراضي  تساوي 16 ميغا بايت.
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

يقوم بتهيئة مثيل جديد لملف[`LzmaCompressionSettings`](../)فئة بحجم القاموس الافتراضي ، تساوي 16 ميغا بايت.

```csharp
public LzmaCompressionSettings()
```

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [LzmaCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* المجسم [Aspose.Zip](../../../)


