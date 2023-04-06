---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipPPMdCompressionSettings नर्मत. 7z आर्कइव के भतर PPMd कम्प्रेशन वध के लए सेटंग्स क इंस्टैंट करत है
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

7z आर्काइव के भीतर PPMd कम्प्रेशन विधि के लिए सेटिंग्स को इंस्टैंट करता है।

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| maxOrder | Byte | अधिकतम आदेश। |
| suballocatorSize | Int32 | एमबी सबऑलोकेटर में मेमोरी का आकार खपत कर सकता है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* 2 और 32 के बीच नहीं है, या*suballocatorSize* 1 और 1024 के बीच नहीं है। |

### टिप्पणियों

बड़ा मॉडल ऑर्डर लगभग निश्चित रूप से बेहतर संपीड़न और निश्चित रूप से अधिक मेमोरी और सीपीयू उपयोग का परिणाम है।

PPMd एल्गोरिथ्म को बहुत अधिक मेमोरी की आवश्यकता हो सकती है, विशेष रूप से जब बड़ी फ़ाइलों पर उपयोग किया जाता है और/या बड़े मॉडल ऑर्डर के साथ उपयोग किया जाता है।

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### यह सभी देखें

* class [SevenZipPPMdCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* सभा [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

डिफ़ॉल्ट मॉडल क्रम और उप-आवंटन आकार के साथ 7z संग्रह के भीतर PPMd संपीड़न विधि के लिए सेटिंग्स को त्वरित करता है।

```csharp
public SevenZipPPMdCompressionSettings()
```

### टिप्पणियों

डिफ़ॉल्ट मॉडल क्रम 6 है और सब-एलोकेटर का आकार 16 एमबी है।

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### यह सभी देखें

* class [SevenZipPPMdCompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* सभा [Aspose.Zip](../../../)


