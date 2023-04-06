---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: LzmaCompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैLzmaCompressionSettingsडफल्ट डक्शनर सइज वल क्लस 16 मेगबइट के बरबर हत है
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

का एक नया उदाहरण प्रारंभ करता है[`LzmaCompressionSettings`](../)डिफॉल्ट डिक्शनरी साइज वाली क्लास, 16 मेगाबाइट के बराबर होती है।

```csharp
public LzmaCompressionSettings()
```

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [LzmaCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* सभा [Aspose.Zip](../../../)


