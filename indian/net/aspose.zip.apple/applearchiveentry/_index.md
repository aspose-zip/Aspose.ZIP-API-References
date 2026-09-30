---
title: "क्लास AppleArchiveEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Apple.AppleArchiveEntry class. AppleArchive के भीतर फ़ाइल‑सिस्टम प्रविष्टि का प्रतिनिधित्व करता है"
type: docs
weight: 70
url: /hi/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

[`AppleArchive`](../applearchive/) के भीतर फ़ाइल‑सिस्टम प्रविष्टि का प्रतिनिधित्व करता है।

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टि एक निर्देशिका का प्रतिनिधित्व करती है या नहीं। |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टि एक सिम्बॉलिक लिंक का प्रतिनिधित्व करती है या नहीं। |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | प्रविष्टि की अनकम्प्रेस्ड लंबाई बाइट्स में प्राप्त करता है। |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | आर्काइव के भीतर प्रविष्टि का पथ प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | प्रदान की गई स्ट्रीम में एंट्री को एक्सट्रैक्ट करता है। |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | प्रदान किए गए पाथ द्वारा फ़ाइल सिस्टम में एंट्री को एक्सट्रैक्ट करता है। |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |

## टिप्पणियाँ

इस क्लास का एक उदाहरण मौजूदा Apple Archive से पार्स की गई नियमित फ़ाइल, निर्देशिका, या सिम्बॉलिक लिंक का प्रतिनिधित्व कर सकता है, या निर्मित हो रहे आर्काइव में जोड़ी गई फ़ाइल या निर्देशिका का।

### संबंधित देखें

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


