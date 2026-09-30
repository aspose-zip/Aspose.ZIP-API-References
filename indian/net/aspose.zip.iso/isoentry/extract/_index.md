---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoEntry मेथड। प्रदान किए गए पथ के अनुसार एंट्री को फ़ाइल सिस्टम में एक्सट्रैक्ट करता है"
type: docs
weight: 50
url: /hi/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है।

```csharp
public FileInfo Extract(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | डेस्टिनेशन फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे ओवरराइट कर दिया जाएगा। |

### रिटर्न वैल्यू

FileInfo इंस्टेंस जिसमें एक्सट्रैक्ट किया गया डेटा होता है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| InvalidOperationException | आर्काइव हेडर्स और सर्विस जानकारी पढ़ी नहीं गई। |

### संबंधित देखें

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

प्रदान की गई स्ट्रीम में एंट्री को एक्सट्रैक्ट करता है।

```csharp
public void Extract(Stream destination)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| डेस्टिनेशन | स्ट्रीम | डेस्टिनेशन स्ट्रीम। लिखने योग्य होना चाहिए। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| NotSupportedException | यदि एंट्री फ़ाइल का प्रतिनिधित्व नहीं करती है तो यह त्रुटि उत्पन्न करता है। |
| ArgumentException | प्रदान की गई स्ट्रीम लिखने का समर्थन नहीं करती है। |

### संबंधित देखें

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


