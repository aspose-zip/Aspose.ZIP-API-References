---
title: WimImage.ExtractToDirectory
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: WimImage तरक. इमेज क सभ फइलं क प्रदन क गई डयरेक्टर में नकलत है
type: docs
weight: 40
url: /hi/net/aspose.zip.wim/wimimage/extracttodirectory/
---
## WimImage.ExtractToDirectory method

इमेज की सभी फाइलों को प्रदान की गई डायरेक्टरी में निकालता है।

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | String | निकाली गई फ़ाइलों को रखने के लिए निर्देशिका का पथ। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | पथ शून्य है |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| SecurityException | कॉल करने वाले के पास मौजूदा निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| NotSupportedException | यदि निर्देशिका मौजूद नहीं है, तो पथ में एक बृहदान्त्र वर्ण (:) होता है जो ड्राइव लेबल ("C: \") का हिस्सा नहीं होता है। |
| ArgumentException | पथ एक शून्य-लंबाई वाली स्ट्रिंग है, जिसमें केवल सफेद स्थान है, या एक या अधिक अमान्य वर्ण हैं। आप System.IO.Path.GetInvalidPathChars पद्धति का उपयोग करके अमान्य वर्णों के लिए क्वेरी कर सकते हैं। -या- पथ के साथ उपसर्ग है, या केवल एक बृहदान्त्र वर्ण (:) है। |
| IOException | पथ द्वारा निर्दिष्ट निर्देशिका एक फ़ाइल है। -या- नेटवर्क का नाम ज्ञात नहीं है। |

### टिप्पणियों

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

### उदाहरण

```csharp
using (var archive = new WimArchive("install.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### यह सभी देखें

* class [WimImage](../)
* नाम स्थान [Aspose.Zip.Wim](../../wimimage/)
* सभा [Aspose.Zip](../../../)

