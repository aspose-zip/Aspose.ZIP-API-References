---
title: "XarArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarArchive मेथड। प्रदान की गई गंतव्य फ़ाइल में संग्रह को सहेजता है।"
type: docs
weight: 80
url: /hi/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

प्रदान किए गए गंतव्य फ़ाइल में अभिलेख सहेजता है।

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| saveOptions | XarSaveOptions | xar संग्रह को सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य (null) है। |
| InvalidOperationException | xar संग्रह को संशोधित करना असंभव है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। |
| UnauthorizedAccessException | *destinationFileName* ने एक पढ़ने-केवल फ़ाइल निर्दिष्ट की। -या- *destinationFileName* ने एक निर्देशिका निर्दिष्ट की। -या- कॉलर के पास आवश्यक अनुमति नहीं है। |

### संबंधित देखें

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |
| saveOptions | XarSaveOptions | xar संग्रह को सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *output* लिखने योग्य नहीं है। |
| ArgumentException | *output* लिखने/पढ़ने योग्य नहीं है या खोज योग्य नहीं है। |
| InvalidOperationException | xar संग्रह को संशोधित करना असंभव है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

### संबंधित देखें

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


