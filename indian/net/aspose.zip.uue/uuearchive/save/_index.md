---
title: "UueArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "UueArchive मेथड। प्रदान की गई स्ट्रीम में अभिलेख को सहेजता है"
type: docs
weight: 70
url: /hi/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| outputStream | स्ट्रीम | गंतव्य स्ट्रीम। |
| saveOptions | UueSaveOptions | अभिलेख सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | अभिलेखित किए जाने वाले डेटा का स्रोत प्रदान नहीं किया गया है। |
| ArgumentException | *outputStream* लिखने योग्य नहीं है। |
| UnauthorizedAccessException | फ़ाइल स्रोत केवल-पढ़ने योग्य है या यह एक डायरेक्टरी है। |
| DirectoryNotFoundException | निर्दिष्ट फ़ाइल स्रोत पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर हो। |
| IOException | फ़ाइल स्रोत पहले ही खुला हुआ है। |

## टिप्पणियाँ

*outputStream* must be writable.

## उदाहरण

संपीड़ित डेटा को http प्रतिक्रिया स्ट्रीम में लिखें।

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### संबंधित देखें

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

आर्काइव को प्रदान की गई गंतव्य फ़ाइल में सहेजता है।

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| saveOptions | UueSaveOptions | अभिलेख सहेजने के विकल्प। |

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
| InvalidOperationException | अभिलेखित किए जाने वाले डेटा का स्रोत प्रदान नहीं किया गया है। |

## उदाहरण

एन्कोडेड डेटा को फ़ाइल में लिखें।

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### संबंधित देखें

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


