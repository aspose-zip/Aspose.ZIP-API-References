---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Lz4Archive मेथड। अभिलेख को पथ द्वारा फ़ाइल में निकालता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

आर्काइव को पथ द्वारा फ़ाइल में निकालता है।

```csharp
public FileInfo Extract(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | डेस्टिनेशन फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे ओवरराइट कर दिया जाएगा। |

### रिटर्न वैल्यू

निकाली गई फ़ाइल की जानकारी।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| EndOfStreamException | स्रोत स्ट्रीम बहुत छोटी है। |
| InvalidDataException | डिकोडिंग के दौरान गलत बाइट्स पाए गए। |
| NotSupportedException | यह LZ4 संस्करण समर्थित नहीं है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | आर्काइव को संयोजन के लिए तैयार किया गया है। |

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है।

```csharp
public void Extract(Stream destination)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| डेस्टिनेशन | स्ट्रीम | डेस्टिनेशन स्ट्रीम। लिखने योग्य होना चाहिए। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | *destination* लिखना समर्थन नहीं करता। |
| EndOfStreamException | स्रोत स्ट्रीम बहुत छोटी है। |
| InvalidDataException | डिकोडिंग के दौरान गलत बाइट्स पाए गए। |
| NotSupportedException | यह LZ4 संस्करण समर्थित नहीं है। |
| InvalidOperationException | आर्काइव को संयोजन के लिए तैयार किया गया है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


