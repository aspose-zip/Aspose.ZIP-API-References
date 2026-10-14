---
title: "AlzArchive.ExtractToDirectory"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AlzArchive मेथड। आर्काइव में सभी फ़ाइलों और डायरेक्टरीज़ को प्रदान किए गए डायरेक्टरी में एक्सट्रैक्ट करता है।"
type: docs
weight: 40
url: /hi/net/aspose.zip.alz/alzarchive/extracttodirectory/
---
## AlzArchive.ExtractToDirectory method

आर्काइव में सभी फ़ाइलों और डायरेक्टरीज़ को प्रदान की गई डायरेक्टरी में निकालता है।

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationDirectory | String | निकाले गए फ़ाइलों को रखने के लिए निर्देशिका का पथ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *destinationDirectory* null है। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम द्वारा निर्धारित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| SecurityException | कॉलर के पास मौजूदा निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| NotSupportedException | यदि डायरेक्टरी मौजूद नहीं है, तो पथ में कोलन अक्षर (:) हो सकता है जो ड्राइव लेबल ("C:\") का हिस्सा नहीं है। |
| ArgumentException | *destinationDirectory* शून्य-लंबाई की स्ट्रिंग है, केवल खाली स्थान रखती है, या एक या अधिक अमान्य अक्षर शामिल है। आप System.IO.Path.GetInvalidPathChars मेथड का उपयोग करके अमान्य अक्षरों की जाँच कर सकते हैं। -or- पथ केवल कोलन अक्षर (:) से शुरू है या उसमें केवल कोलन अक्षर है। |
| IOException | पथ द्वारा निर्दिष्ट निर्देशिका एक फ़ाइल है। -or- नेटवर्क नाम ज्ञात नहीं है। |
| InvalidDataException | गलत पासवर्ड प्रदान किया गया है। - या - आर्काइव भ्रष्ट है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | जब ऑब्जेक्ट को डिस्पोज़ किया गया हो तब थ्रो किया जाता है। |

## टिप्पणियाँ

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

## उदाहरण

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### संबंधित देखें

* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


