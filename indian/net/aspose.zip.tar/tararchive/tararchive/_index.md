---
title: TarArchive.TarArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैTarArchive वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`TarArchive`](../) वर्ग.

```csharp
public TarArchive()
```

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी फ़ाइल को कैसे कंप्रेस करना है।

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Archive`](../../../aspose.zip/archive/) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public TarArchive(Stream sourceStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। यह खोजने योग्य होना चाहिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidDataException | *sourceStream* खोजने योग्य नहीं है। |

### टिप्पणियों

यह कन्स्ट्रक्टर किसी प्रविष्टि को अनपैक नहीं करता है। देखना[`Open`](../../tarentry/open/)अनपॅकिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी निर्देशिका में सभी प्रविष्टियाँ कैसे निकालें।

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`TarArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public TarArchive(string path)
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

यह कन्स्ट्रक्टर किसी प्रविष्टि को अनपैक नहीं करता है। देखना[`Open`](../../tarentry/open/)अनपॅकिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी निर्देशिका में सभी प्रविष्टियाँ कैसे निकालें।

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


