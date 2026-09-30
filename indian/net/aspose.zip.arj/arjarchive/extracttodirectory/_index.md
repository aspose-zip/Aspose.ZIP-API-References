---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ArjArchive मेथड। सभी एंट्रीज़ को निर्दिष्ट डायरेक्टरी में एक्सट्रैक्ट करता है।"
type: docs
weight: 60
url: /hi/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

सभी एंट्रीज़ को निर्दिष्ट डायरेक्ट्री में एक्सट्रैक्ट करता है।

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationDirectory | String | डायरेक्टरी जहाँ एंट्रीज़ निकाली जाएँगी। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | जब *destinationDirectory* null हो, तब फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| InvalidDataException | हेडर या डेटा के लिए चेकसम मेल नहीं खाता। - या - आर्काइव भ्रष्ट है। |
| NotImplementedException | एंट्री मेथड 4 के साथ संकुचित है। |

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को डायरेक्टरी में कैसे निकाला जाए:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### संबंधित देखें

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


