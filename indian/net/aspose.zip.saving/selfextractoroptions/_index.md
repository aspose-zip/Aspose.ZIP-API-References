---
title: Class SelfExtractorOptions
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Saving.SelfExtractorOptions कक्ष. स्वनष्कर्षण नष्पदन यग्य संग्रह के नर्मण के लए वकल्प
type: docs
weight: 500
url: /hi/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

स्व-निष्कर्षण निष्पादन योग्य संग्रह के निर्माण के लिए विकल्प।

```csharp
public class SelfExtractorOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि निकासी पर एक्सट्रैक्टर विंडो बंद होनी चाहिए या नहीं। |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | एक्सट्रैक्टर की विंडो का शीर्षक प्राप्त या सेट करता है। |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | संग्रह निष्कर्षण पूरा होने के बाद निष्पादित होने वाले प्रोग्राम को प्राप्त या सेट करता है। |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | एक्सट्रैक्टर एप्लिकेशन की मुख्य विंडो के लिए शीर्षक आइकन के लिए पथ प्राप्त या सेट करता है। |

### टिप्पणियों

सेल्फ-एक्सट्रैक्टिंग आर्काइव को मीटर्ड लाइसेंस के साथ नहीं बनाया जा सकता है:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### उदाहरण

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### यह सभी देखें

* नाम स्थान [Aspose.Zip.Saving](../../aspose.zip.saving/)
* सभा [Aspose.Zip](../../)


