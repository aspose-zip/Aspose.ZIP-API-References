---
title: Archive.ExtractToDirectory
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive तरक. संग्रह क सभ फइलं क प्रदन क गई नर्देशक में नकलत है
type: docs
weight: 80
url: /hi/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

संग्रह की सभी फाइलों को प्रदान की गई निर्देशिका में निकालता है।

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | String | निकाली गई फ़ाइलों को रखने के लिए निर्देशिका का पथ। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *destinationDirectory* शून्य है। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| SecurityException | कॉल करने वाले के पास मौजूदा निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| NotSupportedException | यदि निर्देशिका मौजूद नहीं है, तो पथ में एक बृहदान्त्र वर्ण (:) होता है जो ड्राइव लेबल ("C: \") का हिस्सा नहीं होता है। |
| ArgumentException | *destinationDirectory*एक शून्य-लंबाई वाली स्ट्रिंग है, जिसमें केवल सफेद स्थान है, या एक या अधिक अमान्य वर्ण हैं। आप System.IO.Path.GetInvalidPathChars पद्धति का उपयोग करके अमान्य वर्णों के लिए क्वेरी कर सकते हैं। -या- पथ के साथ उपसर्ग है, या इसमें केवल एक बृहदान्त्र वर्ण (:) है। |
| IOException | पथ द्वारा निर्दिष्ट निर्देशिका एक फ़ाइल है। -या- नेटवर्क का नाम ज्ञात नहीं है। |
| InvalidDataException | गलत पासवर्ड दिया गया है। |

### टिप्पणियों

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

### उदाहरण

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### यह सभी देखें

* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


