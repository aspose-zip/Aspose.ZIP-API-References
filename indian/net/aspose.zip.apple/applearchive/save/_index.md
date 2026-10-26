---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchive मेथड। प्रदान किए गए स्ट्रीम में अभिलेख को सहेजता है।"
type: docs
weight: 90
url: /hi/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream output)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | संग्रह को नष्ट कर दिया गया है। |
| ArgumentNullException | *output* `null` है। |
| ArgumentException | आर्काइव निकासी के लिए तैयार है। - या - स्रोत प्रदान नहीं किया गया था। |
| ArgumentOutOfRangeException | कॉन्फ़िगर किया गया LZ4 या Zlib ब्लॉक आकार सकारात्मक नहीं है। |
| NotSupportedException | कम्प्रेशन सेटिंग्स गायब या असमर्थित हैं, प्रत्यक्ष निर्माण एक गैर-सीक करने योग्य स्ट्रीम का उपयोग करता है, या एंट्री/अभिलेख आकार वर्तमान Apple Archive सीमाओं से अधिक है। |

## टिप्पणियाँ

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### संबंधित देखें

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

आर्काइव को प्रदान की गई गंतव्य फ़ाइल में सहेजता है।

```csharp
public void Save(string destinationFileName)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | निर्माण के लिए अभिलेख का पथ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | संग्रह को नष्ट कर दिया गया है। |
| ArgumentException | *destinationFileName* अमान्य है। |
| ArgumentNullException | *destinationFileName* `null` है। |
| ArgumentOutOfRangeException | कॉन्फ़िगर किया गया LZ4 या Zlib ब्लॉक आकार सकारात्मक नहीं है। |
| NotSupportedException | कम्प्रेशन सेटिंग्स गायब या असमर्थित हैं, प्रत्यक्ष निर्माण एक गैर-सीक करने योग्य स्ट्रीम का उपयोग करता है, या एंट्री/अभिलेख आकार वर्तमान Apple Archive सीमाओं से अधिक है। |

### संबंधित देखें

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


