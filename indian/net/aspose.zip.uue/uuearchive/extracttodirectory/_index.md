---
title: "UueArchive.ExtractToDirectory"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "UueArchive मेथड। अभिलेख की सामग्री को प्रदान की गई डायरेक्टरी में निकालता है।"
type: docs
weight: 50
url: /hi/net/aspose.zip.uue/uuearchive/extracttodirectory/
---
## UueArchive.ExtractToDirectory method

आर्काइव की सामग्री को प्रदान किए गए डायरेक्टरी में निकालता है।

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationDirectory | String | निकाले गए फ़ाइलों को रखने के लिए निर्देशिका का पथ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | *destinationDirectory* null है। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम द्वारा निर्धारित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| SecurityException | कॉलर के पास मौजूदा निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| NotSupportedException | यदि डायरेक्टरी मौजूद नहीं है, तो पथ में कोलन अक्षर (:) हो सकता है जो ड्राइव लेबल ("C:\") का हिस्सा नहीं है। |
| ArgumentException | *destinationDirectory* शून्य-लंबाई की स्ट्रिंग है, केवल खाली स्थान रखती है, या एक या अधिक अमान्य अक्षर शामिल है। आप System.IO.Path.GetInvalidPathChars मेथड का उपयोग करके अमान्य अक्षरों की जाँच कर सकते हैं। -or- पथ केवल कोलन अक्षर (:) से शुरू है या उसमें केवल कोलन अक्षर है। |
| IOException | पथ द्वारा निर्दिष्ट निर्देशिका एक फ़ाइल है। -or- नेटवर्क नाम ज्ञात नहीं है। |

## टिप्पणियाँ

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


