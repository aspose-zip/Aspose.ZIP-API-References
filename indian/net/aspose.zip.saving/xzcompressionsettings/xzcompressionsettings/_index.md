---
title: XzCompressionSettings.XzCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: XzCompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैXzCompressionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

का एक नया उदाहरण प्रारंभ करता है[`XzCompressionSettings`](../) वर्ग.

```csharp
public XzCompressionSettings()
```

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [XzCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../xzcompressionsettings/)
* सभा [Aspose.Zip](../../../)


