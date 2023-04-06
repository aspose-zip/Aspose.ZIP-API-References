---
title: SevenZipArchive.SaveSplit
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchive तरक. मल्टवल्यूम संग्रह प्रदन क गई गंतव्य नर्देशक में सहेजत है
type: docs
weight: 90
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

मल्टी-वॉल्यूम संग्रह प्रदान की गई गंतव्य निर्देशिका में सहेजता है।

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | String | उस निर्देशिका का पथ जहां संग्रह खंड बनाए जाने हैं। |
| options | SplitSevenZipArchiveSaveOptions | फ़ाइल नाम सहित संग्रह सहेजने के विकल्प। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | यह संग्रह मौजूदा स्रोत से खोला गया था। |
| ArgumentNullException | *destinationDirectory* शून्य है। |
| SecurityException | कॉल करने वाले के पास निर्देशिका तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationDirectory* में अमान्य वर्ण हैं जैसे ",&gt;, &lt;, या &#x7C;। |
| PathTooLongException | निर्दिष्ट पथ सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। |

### टिप्पणियों

यह विधि कई रचना (`एन`) फ़ाइल नाम.7z.001, फ़ाइलनाम.7z.002, ..., फ़ाइलनाम.7z.(एन).

मौजूदा संग्रह को बहु-वॉल्यूम नहीं बनाया जा सकता.

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### यह सभी देखें

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)


