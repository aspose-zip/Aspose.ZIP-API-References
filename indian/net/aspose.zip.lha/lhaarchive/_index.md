---
title: "क्लास LhaArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Lha.LhaArchive क्लास। यह क्लास एक LHA .lzh आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 630
url: /hi/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

यह क्लास एक LHA (.lzh) आर्काइव फ़ाइल का प्रतिनिधित्व करती है।

```csharp
public class LhaArchive : IArchive
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | नया `LhaArchive` क्लास का इंस्टेंस प्रारंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | नया `LhaArchive` क्लास का इंस्टेंस प्रारंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | आर्काइव बनाते हुए [`LhaArchiveEntry`](../lhaarchiveentry/) प्रकार की फ़ाइल एंट्रीज़ प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | आर्काइव में सभी फ़ाइलों और डायरेक्टरीज़ को प्रदान की गई डायरेक्टरी में निकालता है। |

## टिप्पणियाँ

केवल निम्नलिखित संपीड़न विधियों का समर्थन किया जाता है:

**Method**

**Explanation**

**lh0**

असंपीड़ित

**lh4**

8 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman

**lh5**

16 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman

**lh6**

64 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman

**lh7**

128 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman

**lhx**

1 Mib स्लाइडिंग डिक्शनरी और स्थिर Huffman

**lhd**

डायरेक्टरी

### संबंधित देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


