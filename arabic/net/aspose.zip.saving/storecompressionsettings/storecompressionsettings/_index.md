---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: StoreCompressionSettings البناء. يقوم بتهيئة مثيل جديد لملفStoreCompressionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

يقوم بتهيئة مثيل جديد لملف[`StoreCompressionSettings`](../) فئة .

```csharp
public StoreCompressionSettings()
```

### أمثلة

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [StoreCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../storecompressionsettings/)
* المجسم [Aspose.Zip](../../../)


