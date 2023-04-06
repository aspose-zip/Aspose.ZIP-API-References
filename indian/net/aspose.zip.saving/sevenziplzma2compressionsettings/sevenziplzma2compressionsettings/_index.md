---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipLZMA2CompressionSettings नर्मत. 7z संग्रह के भतर LZMA2 संपड़न वध के लए सेटंग्स क त्वरत करत है
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

7z संग्रह के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को त्वरित करता है।

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dictionarySize | Int32 | इतिहास बफ़र का आकार, 4096 और 1073741824 के बीच होना चाहिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* बहुत बड़ा या बहुत छोटा है। |

### टिप्पणियों

डिक्शनरी जितनी बड़ी होगी, कंप्रेशन अनुपात उतना ही बेहतर होगा, लेकिन असम्पीडित डेटा से बड़े डिक्शनरी रैम की बर्बादी हैं।

### यह सभी देखें

* class [SevenZipLZMA2CompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* सभा [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

7z संग्रह के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को त्वरित करता है।

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dictionarySize | Int32 | इतिहास बफ़र का आकार, 4096 और 1073741824 के बीच होना चाहिए। |
| fastBytes | Int32 | LZMA2 कम्प्रेसर द्वारा उपयोग किए जाने वाले तेज़ बाइट्स की संख्या को नियंत्रित करता है। तेजी से बाइट्स की एक बड़ी संख्या संपीड़न गति की कीमत पर बेहतर संपीड़न अनुपात प्रदान कर सकती है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* बहुत बड़ा या बहुत छोटा है, या*fastBytes* बहुत बड़ा या बहुत छोटा है। |

### टिप्पणियों

डिक्शनरी जितनी बड़ी होगी, कंप्रेशन अनुपात उतना ही बेहतर होगा, लेकिन असम्पीडित डेटा से बड़े डिक्शनरी रैम की बर्बादी हैं।

### यह सभी देखें

* class [SevenZipLZMA2CompressionSettings](../)
* नाम स्थान [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* सभा [Aspose.Zip](../../../)


