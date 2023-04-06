---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: DeflateCompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैDeflateCompressionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

का एक नया उदाहरण प्रारंभ करता है[`DeflateCompressionSettings`](../) वर्ग.

```csharp
public DeflateCompressionSettings()
```

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [DeflateCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* सभा [Aspose.Zip](../../../)


