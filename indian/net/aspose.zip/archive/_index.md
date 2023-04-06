---
title: Class Archive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Archive कक्ष. यह वर्ग ज़प संग्रह फ़इल क प्रतनधत्व करत है ज़प संग्रह बनने नकलने य अपडेट करने के लए इसक उपयग करें.
type: docs
weight: 10
url: /hi/net/aspose.zip/archive/
---
## Archive class

यह वर्ग ज़िप संग्रह फ़ाइल का प्रतिनिधित्व करता है। ज़िप संग्रह बनाने, निकालने या अपडेट करने के लिए इसका उपयोग करें.

```csharp
public class Archive : IArchive
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | का एक नया उदाहरण प्रारंभ करता है`Archive` इसकी प्रविष्टियों के लिए वैकल्पिक सेटिंग्स के साथ वर्ग। |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | का एक नया उदाहरण प्रारंभ करता है`Archive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | का एक नया उदाहरण प्रारंभ करता है`Archive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | की प्रविष्टियां प्राप्त करता है[`ArchiveEntry`](../archiveentry/) संग्रह का गठन टाइप करें। |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`ArchiveEntry`](../archiveentry/) आइटम. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है। |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है। |
| [Dispose](../../aspose.zip/archive/dispose/)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | संग्रह की सभी फाइलों को प्रदान की गई निर्देशिका में निकालता है। |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | संग्रह को प्रदान की गई स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | मल्टी-वॉल्यूम संग्रह प्रदान की गई गंतव्य निर्देशिका में सहेजता है। |

### यह सभी देखें

* interface [IArchive](../iarchive/)
* नाम स्थान [Aspose.Zip](../../aspose.zip/)
* सभा [Aspose.Zip](../../)


