---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchiveEntry मेथड। प्रदान किए गए पथ द्वारा प्रविष्टि को फ़ाइल सिस्टम में निकालता है"
type: docs
weight: 50
url: /hi/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है।

```csharp
public FileInfo Extract(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | डेस्टिनेशन फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे ओवरराइट कर दिया जाएगा। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidDataException | प्रविष्टि के लिए संग्रहीत चेकसम या डाइजेस्ट निकाले गए डेटा से मेल नहीं खाता। |
| InvalidOperationException | प्रविष्टि एक ऐसी आर्काइव से संबंधित है जो संयोजन के लिए तैयार की गई है, या प्रविष्टि डेटा को गैर-सीक करने योग्य आर्काइव स्ट्रीम से नहीं खोला जा सकता। |
| NotSupportedException | प्रविष्टि एक सॉलिड Apple Archive से संबंधित है या असमर्थित कम्प्रेशन विधि का उपयोग करती है। |
| ObjectDisposedException | स्रोत स्ट्रीम को नष्ट कर दिया गया है। |
| IOException | एक I/O त्रुटि हुई। |

### संबंधित देखें

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
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
| ArgumentNullException | *destination* `null` है। |
| ArgumentException | *destination* लिखना समर्थन नहीं करता। |
| InvalidDataException | प्रविष्टि के लिए संग्रहीत चेकसम या डाइजेस्ट निकाले गए डेटा से मेल नहीं खाता। |
| InvalidOperationException | प्रविष्टि एक ऐसी आर्काइव से संबंधित है जो संयोजन के लिए तैयार की गई है, या प्रविष्टि डेटा को गैर-सीक करने योग्य आर्काइव स्ट्रीम से नहीं खोला जा सकता। |
| NotSupportedException | प्रविष्टि एक सॉलिड Apple Archive से संबंधित है या असमर्थित कम्प्रेशन विधि का उपयोग करती है। |
| ObjectDisposedException | स्रोत स्ट्रीम को नष्ट कर दिया गया है। |
| IOException | एक I/O त्रुटि हुई। |

### संबंधित देखें

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


