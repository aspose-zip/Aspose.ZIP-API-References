---
title: Class SevenZipArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.SevenZip.SevenZipArchive कक्ष. यह वर्ग 7z संग्रह फ़इल क प्रतनधत्व करत है 7z संग्रह बनने और नकलने के लए इसक उपयग करें.
type: docs
weight: 660
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

यह वर्ग 7z संग्रह फ़ाइल का प्रतिनिधित्व करता है। 7z संग्रह बनाने और निकालने के लिए इसका उपयोग करें.

```csharp
public class SevenZipArchive : IArchive
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | का एक नया उदाहरण प्रारंभ करता है`SevenZipArchive` इसकी प्रविष्टियों के लिए वैकल्पिक सेटिंग्स के साथ वर्ग। |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | का एक नया उदाहरण प्रारंभ करता है`SevenZipArchive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | का एक नया उदाहरण प्रारंभ करता है`SevenZipArchive` क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | की प्रविष्टियां प्राप्त करता है[`SevenZipArchiveEntry`](../sevenziparchiveentry/) संग्रह का गठन टाइप करें। |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`SevenZipArchiveEntry`](../sevenziparchiveentry/) आइटम. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | संग्रह में एकल प्रविष्टि बनाएं. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | संग्रह में एकल प्रविष्टि बनाएं. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | संग्रह की सभी फाइलों को प्रदान की गई निर्देशिका में निकालता है। |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | 7z संग्रह को प्रदान की गई स्ट्रीम में सहेजता है. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | मल्टी-वॉल्यूम संग्रह प्रदान की गई गंतव्य निर्देशिका में सहेजता है। |

### यह सभी देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* नाम स्थान [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* सभा [Aspose.Zip](../../)


