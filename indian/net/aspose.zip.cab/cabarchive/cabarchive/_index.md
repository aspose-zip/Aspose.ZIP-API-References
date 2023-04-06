---
title: CabArchive.CabArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: CabArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैCabArchive क्लस और कंपज़ एंट्र लस्ट क आर्कइव से नकल ज सकत है
type: docs
weight: 10
url: /hi/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`CabArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public CabArchive(Stream sourceStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। यह खोजने योग्य होना चाहिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *sourceStream* शून्य है। |
| ArgumentException | *sourceStream* खोजने योग्य नहीं है। |
| InvalidDataException | *sourceStream* मान्य कैब संग्रह नहीं है. |

### टिप्पणियों

यह कन्स्ट्रक्टर किसी प्रविष्टि को अनपैक नहीं करता है। देखना[`Open`](../../cabentry/open/)अनपॅकिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी निर्देशिका में सभी प्रविष्टियाँ कैसे निकालें।

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### यह सभी देखें

* class [CabArchive](../)
* नाम स्थान [Aspose.Zip.Cab](../../cabarchive/)
* सभा [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`CabArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public CabArchive(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | संग्रह फ़ाइल का पथ। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

यह कन्स्ट्रक्टर किसी प्रविष्टि को अनपैक नहीं करता है। देखना[`Open`](../../cabentry/open/)अनपॅकिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी निर्देशिका में सभी प्रविष्टियाँ कैसे निकालें।

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### यह सभी देखें

* class [CabArchive](../)
* नाम स्थान [Aspose.Zip.Cab](../../cabarchive/)
* सभा [Aspose.Zip](../../../)


