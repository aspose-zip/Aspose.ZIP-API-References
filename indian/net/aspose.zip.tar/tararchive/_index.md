---
title: Class TarArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Tar.TarArchive कक्ष. यह वर्ग टर संग्रह फ़इल क प्रतनधत्व करत है टर आर्कइव बनने नकलने य अपडेट करने के लए इसक उपयग करें
type: docs
weight: 730
url: /hi/net/aspose.zip.tar/tararchive/
---
## TarArchive class

यह वर्ग टार संग्रह फ़ाइल का प्रतिनिधित्व करता है। टार आर्काइव बनाने, निकालने या अपडेट करने के लिए इसका उपयोग करें।

```csharp
public class TarArchive : IArchive
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`TarArchive` वर्ग. |
| [TarArchive](tararchive/#constructor_1)(Stream) | का एक नया उदाहरण प्रारंभ करता है[`Archive`](../../aspose.zip/archive/) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |
| [TarArchive](tararchive/#constructor_2)(string) | का एक नया उदाहरण प्रारंभ करता है`TarArchive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | की प्रविष्टियां प्राप्त करता है[`TarEntry`](../tarentry/) संग्रह का गठन टाइप करें। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | आपूर्ति किए गए gzip आर्काइव को निकालता है और बनाता है`TarArchive` निकाले गए डेटा से. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | आपूर्ति किए गए gzip आर्काइव को निकालता है और बनाता है`TarArchive` निकाले गए डेटा से. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | दिए गए अर्क lzip आर्काइव और कंपोज़ करते हैं`TarArchive` निकाले गए डेटा से. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | दिए गए अर्क lzip आर्काइव और कंपोज़ करते हैं`TarArchive` निकाले गए डेटा से. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | आपूर्ति किए गए एक्सज़ेड प्रारूप संग्रह को निकालता है और रचना करता है`TarArchive` निकाले गए डेटा से. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | आपूर्ति किए गए एक्सज़ेड प्रारूप संग्रह को निकालता है और रचना करता है`TarArchive` निकाले गए डेटा से. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | एक्सट्रेक्ट्स ने Z फॉर्मेट आर्काइव की आपूर्ति की और रचना की`TarArchive` निकाले गए डेटा से. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | एक्सट्रेक्ट्स ने Z फॉर्मेट आर्काइव की आपूर्ति की और रचना की`TarArchive` निकाले गए डेटा से. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | संग्रह में एकल प्रविष्टि बनाएं. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है। |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है। |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | संग्रह की सभी फाइलों को प्रदान की गई निर्देशिका में निकालता है। |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | संग्रह को प्रदान की गई स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | gzip कम्प्रेशन के साथ संग्रह को स्ट्रीम में सहेजता है. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | आर्काइव को फ़ाइल में gzip कम्प्रेशन के साथ पथ द्वारा सहेजता है. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | संग्रह को lzip कम्प्रेशन के साथ स्ट्रीम में सहेजता है. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | आर्काइव को lzip कम्प्रेशन के साथ फाइल में सहेजता है। |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | संग्रह को xz संपीड़न के साथ स्ट्रीम में सहेजता है. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | संग्रह को xz संपीड़न के साथ पथ द्वारा पथ में सहेजता है. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | आर्काइव को जेड कम्प्रेशन के साथ स्ट्रीम में सेव करता है। |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | आर्काइव को जेड कम्प्रेशन के साथ पाथ बाई पाथ में सेव करता है। |

### यह सभी देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* नाम स्थान [Aspose.Zip.Tar](../../aspose.zip.tar/)
* सभा [Aspose.Zip](../../)


