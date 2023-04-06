---
title: SevenZipArchive.Save
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchive तरक. 7z संग्रह क प्रदन क गई स्ट्रम में सहेजत है.
type: docs
weight: 80
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

7z संग्रह को प्रदान की गई स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream output)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *output* मांगने का समर्थन नहीं करता। |
| ArgumentNullException | *output* शून्य है। |
| InvalidOperationException | एनकोडर डेटा को संपीड़ित करने में विफल रहा। |

### टिप्पणियों

*output* खोजने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है.

```csharp
public void Save(string destinationFileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*destinationFileName* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*destinationFileName* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

एक संग्रह को उसी पथ पर सहेजना संभव है, जिससे इसे लोड किया गया था। हालांकि, इसकी अनुशंसा नहीं की जाती है क्योंकि यह दृष्टिकोण अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

### उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)


