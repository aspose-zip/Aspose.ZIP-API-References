---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SplitArchiveSaveOptions नर्मत. मल्टवल्यूम ज़प संग्रह क सहेजने के लए सेटंग्स क तत्कल करत है
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

मल्टी-वॉल्यूम ज़िप संग्रह को सहेजने के लिए सेटिंग्स को तत्काल करता है।

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | वॉल्यूम के लिए नाम। ज़िप एक्सटेंशन के साथ या उसके बिना हो सकता है। |
| segmentSize | UInt32 | मात्रा का आकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | खंड का आकार 65536 बाइट्स से कम है। |

### टिप्पणियों

कुछ आयतन इससे कम हो सकते हैं*segmentSize*. ज्यादातर मामलों में अंतिम खंड कम होगा लेकिन शायद ही कभी नियमित खंड भी हो सकते हैं।

फाइलों के नाम इस प्रकार होंगे:*fileName* .z01,*fileName* .z02, ...,*fileName* जेड (एन -1),*fileName*ज़िप।

### यह सभी देखें

* class [SplitArchiveSaveOptions](../)
* नाम स्थान [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* सभा [Aspose.Zip](../../../)


