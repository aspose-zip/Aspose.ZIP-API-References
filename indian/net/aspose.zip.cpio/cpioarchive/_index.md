---
title: Class CpioArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Cpio.CpioArchive कक्ष. यह वर्ग cpio संग्रह फ़इल क प्रतनधत्व करत है
type: docs
weight: 160
url: /hi/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

यह वर्ग cpio संग्रह फ़ाइल का प्रतिनिधित्व करता है।

```csharp
public class CpioArchive : IArchive
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`CpioArchive` वर्ग. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | का एक नया उदाहरण प्रारंभ करता है`CpioArchive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |
| [CpioArchive](cpioarchive/#constructor_2)(string) | का एक नया उदाहरण प्रारंभ करता है`CpioArchive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | की प्रविष्टियां प्राप्त करता है[`CpioEntry`](../cpioentry/) संग्रह का गठन टाइप करें। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | संग्रह में एकल प्रविष्टि बनाएं. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है। |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है। |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | संग्रह की सभी फाइलों को प्रदान की गई निर्देशिका में निकालता है। |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | संग्रह को प्रदान की गई स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | gzip कम्प्रेशन के साथ संग्रह को स्ट्रीम में सहेजता है. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | आर्काइव को फ़ाइल में gzip कम्प्रेशन के साथ पथ द्वारा सहेजता है. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | संग्रह को xz संपीड़न के साथ स्ट्रीम में सहेजता है. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | संग्रह को xz संपीड़न के साथ पथ द्वारा पथ में सहेजता है. |

### यह सभी देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* नाम स्थान [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* सभा [Aspose.Zip](../../)


