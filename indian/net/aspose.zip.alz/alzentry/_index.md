---
title: "क्लास AlzEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Alz.AlzEntry क्लास। एक ALZ आर्काइव में फ़ाइल एंट्री का प्रतिनिधित्व करता है जिसमें सभी मेटाडेटा शामिल हैं"
type: docs
weight: 30
url: /hi/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

ALZ आर्काइव में सभी मेटाडेटा के साथ एक फ़ाइल प्रविष्टि का प्रतिनिधित्व करता है।

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | फ़ाइल डेटा का संकुचित आकार बाइट्स में। |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | यदि यह एंट्री एक डायरेक्टरी का प्रतिनिधित्व करती है तो true लौटाता है। |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | फ़ाइल नाम (पाथ के बिना)। |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | फ़ाइल डेटा का अनसंकुचित आकार बाइट्स में। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | प्रदान की गई स्ट्रीम में एंट्री को एक्सट्रैक्ट करता है। |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है। |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | एंट्री को एक्सट्रैक्शन के लिए खोलता है और डिकम्प्रेस्ड एंट्री कंटेंट के साथ एक स्ट्रीम प्रदान करता है। |

### संबंधित देखें

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


