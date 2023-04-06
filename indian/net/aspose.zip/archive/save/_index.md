---
title: Archive.Save
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive तरक. संग्रह क प्रदन क गई स्ट्रम में सहेजत है
type: docs
weight: 90
url: /hi/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

संग्रह को प्रदान की गई स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | Stream | गंतव्य धारा। |
| saveOptions | ArchiveSaveOptions | पुरालेख सहेजने के विकल्प। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *outputStream* लिखने योग्य नहीं है। |

### टिप्पणियों

*outputStream*लिखने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### यह सभी देखें

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| saveOptions | ArchiveSaveOptions | पुरालेख सहेजने के विकल्प। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*destinationFileName* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, विंडोज-आधारित प्लेटफॉर्म पर, पथ 248 वर्णों से कम होना चाहिए और फ़ाइल नाम 260 वर्णों से कम होना चाहिए। |
| NotSupportedException | पर फाइल करें*destinationFileName* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

एक संग्रह को उसी पथ पर सहेजना संभव है, जिससे इसे लोड किया गया था। हालांकि, इसकी अनुशंसा नहीं की जाती है क्योंकि यह दृष्टिकोण अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

### उदाहरण

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### यह सभी देखें

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


