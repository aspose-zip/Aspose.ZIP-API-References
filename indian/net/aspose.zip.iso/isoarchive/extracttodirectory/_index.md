---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoArchive मेथड। सभी एंट्रीज़ को निर्दिष्ट डायरेक्टरी में निकालता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

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
| InvalidOperationException | जब संग्रह संपादन मोड में हो, तब फेंका जाता है। |
| ArgumentNullException | जब *destinationDirectory* null हो, तब फेंका जाता है। |
| OperationCanceledException | .NET Framework 4.0 और उससे ऊपर में: प्रदान किए गए कैंसलेशन टोकन द्वारा निष्कर्षण रद्द होने पर फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को डायरेक्टरी में कैसे निकाला जाए:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### संबंधित देखें

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


