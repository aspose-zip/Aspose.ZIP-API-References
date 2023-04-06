---
title: Archive.SaveSplit
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive तरक. मल्टवल्यूम संग्रह प्रदन क गई गंतव्य नर्देशक में सहेजत है
type: docs
weight: 100
url: /hi/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

मल्टी-वॉल्यूम संग्रह प्रदान की गई गंतव्य निर्देशिका में सहेजता है।

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | String | उस निर्देशिका का पथ जहां संग्रह खंड बनाए जाने हैं। |
| options | SplitArchiveSaveOptions | फ़ाइल नाम सहित संग्रह सहेजने के विकल्प। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | यह संग्रह मौजूदा स्रोत से खोला गया था। |
| NotSupportedException | यह संग्रह XZ विधि से संकुचित और एन्क्रिप्टेड दोनों है। |
| ArgumentNullException | *destinationDirectory* शून्य है। |
| SecurityException | कॉल करने वाले के पास निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationDirectory* में अमान्य वर्ण हैं जैसे ",&gt;, &lt;, या &#x7C;। |
| PathTooLongException | निर्दिष्ट पथ सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। |

### टिप्पणियों

यह विधि कई रचना (`एन`) फ़ाइलें फ़ाइलनाम.z01, फ़ाइलनाम.z02, ..., फ़ाइलनाम.z(n-1), फ़ाइलनाम.ज़िप।

मौजूदा संग्रह को बहु-वॉल्यूम नहीं बनाया जा सकता.

### उदाहरण

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### यह सभी देखें

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


