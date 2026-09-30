---
title: "UueArchive.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "UueArchive मेथड। प्रदान किए गए स्ट्रीम में आर्काइव को निकालता है"
type: docs
weight: 40
url: /hi/net/aspose.zip.uue/uuearchive/extract/
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
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentException | *destination* लिखना समर्थन नहीं करता। |

## उदाहरण

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

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

निकाले गए फ़ाइल की जानकारी।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


