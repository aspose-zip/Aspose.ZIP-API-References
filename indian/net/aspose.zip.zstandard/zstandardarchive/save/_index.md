---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZstandardArchive मेथड। प्रदान किए गए स्ट्रीम में आर्काइव को सहेजता है।"
type: docs
weight: 60
url: /hi/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| outputStream | स्ट्रीम | गंतव्य स्ट्रीम। |
| सेटिंग्स | ZstandardSaveOptions | आर्काइव निर्माण के लिए वैकल्पिक सेटिंग्स। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentException | *outputStream* लिखने योग्य नहीं है। |
| InvalidOperationException | स्रोत प्रदान नहीं किया गया है। |

## टिप्पणियाँ

*outputStream* must be writable.

## उदाहरण

संपीड़ित डेटा को http प्रतिक्रिया स्ट्रीम में लिखें।

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### संबंधित देखें

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

प्रदान किए गए गंतव्य फ़ाइल में अभिलेख सहेजता है।

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| सेटिंग्स | ZstandardSaveOptions | आर्काइव निर्माण के लिए वैकल्पिक सेटिंग्स। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | *destinationFileName* शून्य (null) है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल खाली स्थान रखता है, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *destinationFileName* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *destinationFileName* पर फ़ाइल स्ट्रिंग के मध्य में कोलन (:) रखती है। |
| Exception | रनटाइम त्रुटि होने पर फेंका जाता है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, (उदाहरण के लिए, यह अनमैप्ड ड्राइव पर है)। |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |
| InvalidOperationException | स्रोत प्रदान नहीं किया गया है। |

## उदाहरण

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### संबंधित देखें

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

प्रदान किए गए गंतव्य फ़ाइल में अभिलेख सहेजता है।

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| डेस्टिनेशन | FileInfo | कॉलर के पास *destination* खोलने के लिए आवश्यक अनुमति नहीं है। |
| सेटिंग्स | ZstandardSaveOptions | आर्काइव निर्माण के लिए वैकल्पिक सेटिंग्स। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| SecurityException | *destination* null है। |
| ArgumentException | फ़ाइल पथ खाली है या केवल खाली स्थानों को शामिल करता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| UnauthorizedAccessException | फ़ाइल का पथ केवल-पढ़ने योग्य है या यह एक डायरेक्टरी है। |
| ArgumentNullException | *destinationFileName* में निर्दिष्ट फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| InvalidOperationException | स्रोत प्रदान नहीं किया गया है। |

## उदाहरण

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### संबंधित देखें

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


