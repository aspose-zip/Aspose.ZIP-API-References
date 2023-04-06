---
title: Class ParallelOptions
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Saving.ParallelOptions कक्ष. समनंतर संपड़न के लए वकल्प
type: docs
weight: 490
url: /hi/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

समानांतर संपीड़न के लिए विकल्प।

```csharp
public class ParallelOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | डिस्क पर स्वैप किए बिना संपीड़ित प्रविष्टियों को समायोजित करने के लिए उपलब्ध मेगाबाइट्स में स्मृति अनुमान प्राप्त या सेट करता है। यह मान केवल तभी समझ में आता है[`ParallelCompressInMemory`](./parallelcompressinmemory/) सेटिंग चालू हैAuto मोड. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | मूल्य प्राप्त करता है या सेट करता है जो इंगित करता है कि समानांतर दृष्टिकोण का उपयोग कैसे किया जाए। |

### टिप्पणियों

ये विकल्प कई CPU कोर द्वारा एक साथ संपीड़न का प्रबंधन करते हैं।

### उदाहरण

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### यह सभी देखें

* नाम स्थान [Aspose.Zip.Saving](../../aspose.zip.saving/)
* सभा [Aspose.Zip](../../)


