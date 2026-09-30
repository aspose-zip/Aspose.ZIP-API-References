---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LzxArchiveEntry मेथड। Lzx आर्काइव एंट्री को पथ द्वारा फ़ाइल सिस्टम में निकालता है"
type: docs
weight: 80
url: /hi/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

पथ द्वारा Lzx आर्काइव एंट्री को फ़ाइल सिस्टम में एक्सट्रैक्ट करता है।

```csharp
public FileSystemInfo Extract(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | फ़ाइल का पथ जहाँ डिकम्प्रेस्ड डेटा संग्रहीत होगा। |

### रिटर्न वैल्यू

FileSystemInfoInstance जिसमें निकाला गया डेटा है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | आर्काइव हेडर्स और सर्विस जानकारी पढ़ी नहीं गई। |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| InvalidDataException | हेडर या डेटा के लिए चेकसम मेल नहीं खाता। - या - आर्काइव भ्रष्ट है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| NotSupportedException | अमान्य संपीड़न विधि। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| EndOfStreamException | जब स्ट्रीम का अंत अप्रत्याशित रूप से पहुँच जाता है तो यह थ्रो किया जाता है। |

## उदाहरण

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### संबंधित देखें

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
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
| ArgumentException | *destination* लिखना समर्थन नहीं करता। |
| InvalidDataException | हेडर या डेटा के लिए चेकसम मेल नहीं खाता। - या - आर्काइव भ्रष्ट है। |
| ArgumentNullException | गंतव्य स्ट्रीम null है। |
| NotSupportedException | अमान्य संपीड़न विधि। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| EndOfStreamException | जब स्ट्रीम का अंत अप्रत्याशित रूप से पहुँच जाता है तो यह थ्रो किया जाता है। |

### संबंधित देखें

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


