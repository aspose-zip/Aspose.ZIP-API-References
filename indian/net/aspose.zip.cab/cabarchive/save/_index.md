---
title: "CabArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "CabArchive मेथड। प्रदान किए गए स्ट्रीम में आर्काइव को सहेजता है।"
type: docs
weight: 70
url: /hi/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| outputStream | स्ट्रीम | गंतव्य स्ट्रीम। |
| saveOptions | CabSaveOptions | आर्काइव सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | *outputStream* लिखने योग्य और खोज योग्य नहीं है। |
| ObjectDisposedException | आर्काइव नष्ट कर दिया गया है। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और इसे सहेजा नहीं जा सकता। |

## टिप्पणियाँ

*outputStream* must be writable.

## उदाहरण

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### संबंधित देखें

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

प्रदान किए गए गंतव्य फ़ाइल में अभिलेख सहेजता है।

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| saveOptions | CabSaveOptions | आर्काइव सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य (null) है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल खाली स्थान रखता है, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *destinationFileName* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *destinationFileName* पर फ़ाइल स्ट्रिंग के मध्य में कोलन (:) रखती है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए खोला गया है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

एक आर्काइव को उसी पाथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह तरीका अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

## उदाहरण

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### संबंधित देखें

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


