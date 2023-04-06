---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: StoreCompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैStoreCompressionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

का एक नया उदाहरण प्रारंभ करता है[`StoreCompressionSettings`](../) वर्ग.

```csharp
public StoreCompressionSettings()
```

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [StoreCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../storecompressionsettings/)
* सभा [Aspose.Zip](../../../)


