---
title: "क्लास AppleArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.Apple.AppleArchive क्लास। यह क्लास एक Apple Archive .aar फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Apple Archive फ़ाइलों को बनाने के लिए करें।"
type: docs
weight: 60
url: /hi/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

यह क्लास एक Apple Archive (.aar) फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Apple Archive फ़ाइलें बनाने के लिए करें।

```csharp
public class AppleArchive : IArchive
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | `AppleArchive` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसमें निर्मित एंट्रीज़ के लिए उपयोग किए गए सेटिंग्स होते हैं। |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | `AppleArchive` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | `AppleArchive` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | आर्काइव को बनाते हुए एंट्रीज़ प्राप्त करता है। |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | आर्काइव सॉलिड कम्प्रेशन उपयोग करता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। सॉलिड मोड में, सभी एंट्री डेटा एक ही स्ट्रीम के रूप में कम्प्रेस होते हैं और व्यक्तिगत एंट्री एक्सट्रैक्शन उपलब्ध नहीं होता। इसके बजाय [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) का उपयोग करें। |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | नव निर्मित एंट्रीज़ के लिए उपयोग किए गए सेटिंग्स प्राप्त करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | दिए गए डायरेक्टरी में सभी फ़ाइलों और फ़ोल्डरों को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | अनमैनेज्ड रिसोर्सेज़ को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है। |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में एक्सट्रैक्ट करता है। |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | आर्काइव को प्रदान की गई गंतव्य फ़ाइल में सहेजता है। |

## टिप्पणियाँ

Apple और Apple Archive, Apple Inc. के ट्रेडमार्क हैं।

### संबंधित देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


