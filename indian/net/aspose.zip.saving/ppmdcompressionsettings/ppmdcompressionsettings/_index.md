---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: PPMdCompressionSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैPPMdCompressionSettings वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`PPMdCompressionSettings`](../) वर्ग.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| modelOrder | Int32 | मॉडल का क्रम। |
| suballocatorSize | Int32 | एमबी सबऑलोकेटर में मेमोरी का आकार खपत कर सकता है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* 2 और 16 के बीच नहीं है। - या -*suballocatorSize* 1 और 256 के बीच नहीं है। |

### टिप्पणियों

बड़ा मॉडल ऑर्डर लगभग निश्चित रूप से बेहतर संपीड़न और निश्चित रूप से अधिक मेमोरी और सीपीयू उपयोग का परिणाम है।

PPMd एल्गोरिथ्म को बहुत अधिक मेमोरी की आवश्यकता हो सकती है, विशेष रूप से जब बड़ी फ़ाइलों पर उपयोग किया जाता है और/या बड़े मॉडल ऑर्डर के साथ उपयोग किया जाता है।

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [PPMdCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* सभा [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`PPMdCompressionSettings`](../) डिफ़ॉल्ट मॉडल क्रम और उप-आवंटन आकार के साथ वर्ग।

```csharp
public PPMdCompressionSettings()
```

### टिप्पणियों

डिफ़ॉल्ट मॉडल क्रम 8 है और सब-एलोकेटर का आकार 50 एमबी है।

### उदाहरण

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### यह सभी देखें

* class [PPMdCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* सभा [Aspose.Zip](../../../)


