---
title: "क्लास IsoArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Iso.IsoArchive क्लास। एक ISO आर्काइव ISO 9660 का प्रतिनिधित्व करता है"
type: docs
weight: 570
url: /hi/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

एक ISO आर्काइव (ISO 9660) का प्रतिनिधित्व करता है।

```csharp
public sealed class IsoArchive : IArchive
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | `IsoArchive` क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है और नई फ़ाइलों और डायरेक्ट्रीज़ को जोड़ने के लिए एक खाली ISO आर्काइव बनाता है। |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | `IsoArchive` क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | `IsoArchive` क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | आर्काइव बनाते हुए [`IsoEntry`](../isoentry/) प्रकार की एंट्रीज़ प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | ISO इमेज में एक डायरेक्ट्री जोड़ता है। |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | ISO इमेज में एक फ़ाइल जोड़ता है। |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | ISO इमेज में एक फ़ाइल जोड़ता है। |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | ISO इमेज में एक फ़ाइल जोड़ता है। |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | अनमैनेज्ड रिसोर्सेज़ को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है। |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | सभी एंट्रीज़ को निर्दिष्ट डायरेक्ट्री में एक्सट्रैक्ट करता है। |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | ISO इमेज को निर्दिष्ट स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | ISO इमेज को निर्दिष्ट पाथ में सहेजता है। |

### संबंधित देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


