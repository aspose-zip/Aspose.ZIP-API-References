---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LhaArchiveEntry विधि। Lha आर्काइव प्रविष्टि को पथ द्वारा फ़ाइल सिस्टम में निकालता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Lha आर्काइव एंट्री को पथ द्वारा फ़ाइल सिस्टम में निकालता है।

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
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

## उदाहरण

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### संबंधित देखें

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
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
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

## टिप्पणियाँ

डायरेक्टरी प्रविष्टि के लिए कुछ नहीं करता।

### संबंधित देखें

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Lha आर्काइव एंट्री को फ़ाइल में निकालता है।

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
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |

## टिप्पणियाँ

डायरेक्टरी प्रविष्टि के लिए कुछ नहीं करता।

## उदाहरण

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### संबंधित देखें

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


