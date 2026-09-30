---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ArjEntryPlain मेथड। प्रदान किए गए पथ द्वारा एंट्री को फ़ाइल सिस्टम में निकालता है"
type: docs
weight: 40
url: /hi/net/aspose.zip.arj/arjentryplain/extract/
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

संयुक्त फ़ाइल की फ़ाइल जानकारी।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य या खाली है। |
| ObjectDisposedException | यदि आर्काइव को नष्ट कर दिया गया हो तो फेंका जाता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| InvalidDataException | हेडर या डेटा के लिए चेकसम मेल नहीं खाता। - या - आर्काइव भ्रष्ट है। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। |
| NotImplementedException | एंट्री मेथड 4 के साथ संकुचित है। |

## उदाहरण

rar आर्काइव की दो एंट्री निकालें।

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### संबंधित देखें

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

ARJ आर्काइव एंट्री को फ़ाइल में निकालता है।

```csharp
public void Extract(FileInfo fileInfo)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | डिकम्प्रेस्ड डेटा संग्रहीत करने के लिए FileInfo। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | आर्काइव हेडर्स और सर्विस जानकारी पढ़ी नहीं गई। |
| SecurityException | कॉलर के पास *fileInfo* खोलने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | फ़ाइल पथ खाली है या केवल खाली स्थानों को शामिल करता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| UnauthorizedAccessException | फ़ाइल का पथ केवल-पढ़ने योग्य है या यह एक डायरेक्टरी है। |
| ArgumentNullException | *fileInfo* शून्य है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि आर्काइव को नष्ट कर दिया गया हो तो फेंका जाता है। |
| InvalidDataException | हेडर या डेटा के लिए चेकसम मेल नहीं खाता। - या - आर्काइव भ्रष्ट है। |
| NotImplementedException | एंट्री मेथड 4 के साथ संकुचित है। |

## उदाहरण

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### संबंधित देखें

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| NotImplementedException | एंट्री मेथड 4 के साथ संकुचित है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि आर्काइव को नष्ट कर दिया गया हो तो फेंका जाता है। |

### संबंधित देखें

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


