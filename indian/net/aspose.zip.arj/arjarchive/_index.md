---
title: "क्लास ArjArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Arj.ArjArchive क्लास। यह क्लास एक ARJ आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 250
url: /hi/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

यह क्लास एक ARJ आर्काइव फ़ाइल का प्रतिनिधित्व करती है।

```csharp
public class ArjArchive : IArchive
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | `ArjArchive` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | `ArjArchive` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | टिप्पणी प्राप्त करता है। |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | [`ArjEntryPlain`](../arjentryplain/) प्रकार की एंट्रीज़ प्राप्त करता है जो ARJ आर्काइव बनाती हैं। |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | मूल नाम प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | अनमैनेज्ड रिसोर्सेज़ को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है। |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | सभी एंट्रीज़ को निर्दिष्ट डायरेक्ट्री में एक्सट्रैक्ट करता है। |

## टिप्पणियाँ

केवल निम्नलिखित संपीड़न विधियों का समर्थन किया जाता है:

**Method**

**Explanation**

**0**

असंपीड़ित

**1**

LZ77 और अनुकूलनशील Huffman कोडिंग का संयोजन। सर्वोत्तम अनुपात।

**2**

LZ77 और अनुकूलनशील Huffman कोडिंग का संयोजन।

**3**

LZ77 और अनुकूलनशील Huffman कोडिंग का संयोजन। सर्वोत्तम गति।

### संबंधित देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


