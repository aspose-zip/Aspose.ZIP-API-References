---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AlzEntry मेथड। प्रदान किए गए पाथ द्वारा एंट्री को फ़ाइल सिस्टम में एक्सट्रैक्ट करता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है।

```csharp
public FileInfo Extract(string path, string password = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | डेस्टिनेशन फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे ओवरराइट कर दिया जाएगा। |
| पासवर्ड | String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

### रिटर्न वैल्यू

संयुक्त फ़ाइल की फ़ाइल जानकारी।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| InvalidDataException | आर्काइव भ्रष्ट है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |

## उदाहरण

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### संबंधित देखें

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

प्रदान की गई स्ट्रीम में एंट्री को एक्सट्रैक्ट करता है।

```csharp
public void Extract(Stream destination, string password = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| डेस्टिनेशन | स्ट्रीम | डेस्टिनेशन स्ट्रीम। लिखने योग्य होना चाहिए। |
| पासवर्ड | String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | *destination* लिखना समर्थन नहीं करता। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए नहीं खोला गया है। - या - यह एंट्री एक डायरेक्टरी है। |
| InvalidDataException | एंट्री के भीतर गलत डेटा। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |

## उदाहरण

पासवर्ड के साथ ALZ आर्काइव की एक एंट्री को एक्सट्रैक्ट करें।

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### संबंधित देखें

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


