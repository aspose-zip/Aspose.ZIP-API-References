---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SplitSevenZipArchiveSaveOptions नर्मत. मल्टवल्यूम 7z आर्कइव क सेव करने के लए सेटंग्स क इंस्टैंट करत है
type: docs
weight: 10
url: /hi/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

मल्टी-वॉल्यूम 7z आर्काइव को सेव करने के लिए सेटिंग्स को इंस्टैंट करता है।

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | वॉल्यूम के लिए नाम। .7z एक्सटेंशन के साथ या उसके बिना हो सकता है। |
| segmentSize | UInt32 | मात्रा का आकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* 100 से कम है। |

### टिप्पणियों

कुछ आयतन इससे कम हो सकते हैं*segmentSize*. ज्यादातर मामलों में अंतिम खंड कम होगा लेकिन शायद ही कभी नियमित खंड भी हो सकते हैं।

फाइलों के नाम इस प्रकार होंगे:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z। (एन)।

### यह सभी देखें

* class [SplitSevenZipArchiveSaveOptions](../)
* नाम स्थान [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* सभा [Aspose.Zip](../../../)


