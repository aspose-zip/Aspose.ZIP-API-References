---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: DeflateCompressionSettings البناء. يقوم بتهيئة مثيل جديد لملفDeflateCompressionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

يقوم بتهيئة مثيل جديد لملف[`DeflateCompressionSettings`](../) فئة .

```csharp
public DeflateCompressionSettings()
```

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [DeflateCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* المجسم [Aspose.Zip](../../../)


