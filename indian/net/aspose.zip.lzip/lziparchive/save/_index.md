---
title: LzipArchive.Save
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: LzipArchive तरक. lzip संग्रह क द गई स्ट्रम में सहेजत है.
type: docs
weight: 50
url: /hi/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

lzip संग्रह को दी गई स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream outputStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | Stream | गंतव्य धारा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *outputStream* मांगने का समर्थन नहीं करता। |
| ArgumentNullException | *outputStream* शून्य है। |

### टिप्पणियों

*outputStream* खोजने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

lzip संग्रह प्रदान की गई गंतव्य फ़ाइल में सहेजता है.

```csharp
public void Save(string destinationFileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*destinationFileName* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*destinationFileName* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

lzip संग्रह प्रदान की गई गंतव्य फ़ाइल में सहेजता है.

```csharp
public void Save(FileInfo destination)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destination | FileInfo | FileInfo जो गंतव्य स्ट्रीम के रूप में खोला जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| SecurityException | कॉलर के पास खोलने के लिए आवश्यक अनुमति नहीं है*destination*. |
| ArgumentException | फ़ाइल पथ खाली है या केवल सफेद स्थान हैं। |
| FileNotFoundException | फ़ाइल नहीं मिली. |
| UnauthorizedAccessException | फ़ाइल का पथ केवल पढ़ने के लिए है या एक निर्देशिका है। |
| ArgumentNullException | *destination* शून्य है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि मैप न की गई ड्राइव पर होना। |
| IOException | फाइल पहले से ही खुली हुई है। |

### उदाहरण

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)


