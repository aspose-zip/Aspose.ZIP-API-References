---
title: "Lz4Archive मेथड। प्रदान किए गए स्ट्रीम में lz4 आर्काइव को सहेजता है"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "आउटपुट"
type: docs
weight: 60
url: /hi/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

प्रदान किए गए स्ट्रीम में lz4 अभिलेख सहेजता है।

```csharp
public void Save(Stream output)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *output* लिखने योग्य नहीं है। |
| ArgumentException | आर्काइव निकासी के लिए तैयार है। - या - स्रोत प्रदान नहीं किया गया था। |
| InvalidOperationException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन के माध्यम से संपीड़न रद्द होने पर यह अपवाद फेंका जाता है। |
| OperationCanceledException | FileInfo, जिसे गंतव्य स्ट्रीम के रूप में खोला जाएगा। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

*output* must be seekable.

## उदाहरण

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

प्रदान किए गए गंतव्य फ़ाइल में lz4 अभिलेख सहेजता है।

```csharp
public void Save(FileInfo destination)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| डेस्टिनेशन | FileInfo | कॉलर के पास *destination* खोलने के लिए आवश्यक अनुमति नहीं है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| SecurityException | *destination* null है। |
| ArgumentException | फ़ाइल पथ खाली है या केवल खाली स्थानों को शामिल करता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| UnauthorizedAccessException | फ़ाइल का पथ केवल-पढ़ने योग्य है या यह एक डायरेक्टरी है। |
| ArgumentNullException | *destinationFileName* में निर्दिष्ट फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| InvalidOperationException | आर्काइव को एक्सट्रैक्शन के लिए तैयार किया गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

प्रदान किए गए गंतव्य फ़ाइल में अभिलेख सहेजता है।

```csharp
public void Save(string destinationFileName)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य (null) है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है |
| ArgumentException | *destinationFileName* खाली है, केवल खाली स्थान रखता है, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *destinationFileName* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *destinationFileName* पर फ़ाइल स्ट्रिंग के मध्य में कोलन (:) रखती है। |
| InvalidOperationException | आर्काइव को एक्सट्रैक्शन के लिए तैयार किया गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, (उदाहरण के लिए, यह अनमैप्ड ड्राइव पर है)। |
| FileNotFoundException | Lz4Archive.Lz4Archive |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |

## उदाहरण

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


