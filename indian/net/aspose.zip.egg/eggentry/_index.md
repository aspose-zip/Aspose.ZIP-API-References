---
title: "क्लास EggEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Egg.EggEntry class. EGG आर्काइव में सभी मेटाडेटा के साथ फ़ाइल एंट्री का प्रतिनिधित्व करता है"
type: docs
weight: 470
url: /hi/net/aspose.zip.egg/eggentry/
---
## EggEntry class

EGG आर्काइव में सभी मेटाडेटा के साथ एक फ़ाइल प्रविष्टि का प्रतिनिधित्व करता है।

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | एंट्री का संकुचित आकार प्राप्त करता है। |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह एंट्री एक डायरेक्टरी का प्रतिनिधित्व करती है या नहीं। |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | अंतिम संशोधित तिथि और समय प्राप्त करता है या सेट करता है। |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | आर्काइव के भीतर एंट्री का नाम प्राप्त करता है। |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | एंट्री का अनसंकुचित आकार प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | प्रदान की गई स्ट्रीम में एंट्री को एक्सट्रैक्ट करता है। |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है। |
| [Open](../../aspose.zip.egg/eggentry/open/)() | एंट्री को एक्सट्रैक्शन के लिए खोलता है और डिकम्प्रेस्ड एंट्री कंटेंट के साथ एक स्ट्रीम प्रदान करता है। |

### संबंधित देखें

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


