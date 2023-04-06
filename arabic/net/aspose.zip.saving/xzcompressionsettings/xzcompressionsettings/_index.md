---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: XzCompressionSettings البناء. يقوم بتهيئة مثيل جديد لملفXzCompressionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

يقوم بتهيئة مثيل جديد لملف[`XzCompressionSettings`](../) فئة .

```csharp
public XzCompressionSettings()
```

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [XzCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../xzcompressionsettings/)
* المجسم [Aspose.Zip](../../../)


