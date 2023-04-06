---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2CompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैBzip2CompressionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2CompressionSettings`](../) वर्ग.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | Int32 | सैकड़ों किलोबाइट में ब्लॉक का आकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | ब्लॉक का आकार 1 और 9 के बीच नहीं है। |

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [Bzip2CompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* सभा [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2CompressionSettings`](../) वर्ग डिफ़ॉल्ट ब्लॉक आकार के साथ, 9 सौ किलोबाइट के बराबर.

```csharp
public Bzip2CompressionSettings()
```

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [Bzip2CompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* सभा [Aspose.Zip](../../../)


