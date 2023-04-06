---
title: TarArchive.Save
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. संग्रह क प्रदन क गई स्ट्रम में सहेजत है
type: docs
weight: 120
url: /hi/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

संग्रह को प्रदान की गई स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *output* लिखने योग्य नहीं है। - या -*output* एक ही स्ट्रीम है जिससे हम निकालते हैं. - या - इसमें संग्रह को सहेजना असंभव है*format* प्रारूप प्रतिबंधों के कारण। |

### टिप्पणियों

*output*लिखने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *destinationFileName* एक शून्य-लंबाई वाली स्ट्रिंग है, जिसमें केवल सफेद स्थान है, या System.IO.Path.InvalidPathChars द्वारा परिभाषित एक या अधिक अमान्य वर्ण हैं। |
| ArgumentNullException | *destinationFileName* शून्य है। |
| PathTooLongException | विष्तृत*destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| DirectoryNotFoundException | विष्तृत*destinationFileName* अमान्य है, (उदाहरण के लिए, यह एक अनमैप्ड ड्राइव पर है)। |
| IOException | फ़ाइल खोलते समय I/O त्रुटि हुई। |
| UnauthorizedAccessException | *destinationFileName* एक फ़ाइल निर्दिष्ट की गई है जो केवल पढ़ने के लिए है और पहुंच रीड नहीं है.-या- पथ एक निर्देशिका निर्दिष्ट करता है.-या- कॉलर के पास आवश्यक अनुमति नहीं है। |
| NotSupportedException | *destinationFileName* अमान्य प्रारूप में है। |

### टिप्पणियों

एक संग्रह को उसी पथ पर सहेजना संभव है, जिससे इसे लोड किया गया था। हालांकि, इसकी अनुशंसा नहीं की जाती है क्योंकि यह दृष्टिकोण अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

### उदाहरण

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


