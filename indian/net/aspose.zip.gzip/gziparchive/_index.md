---
title: Class GzipArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Gzip.GzipArchive कक्ष. यह वर्ग gzip संग्रह फ़इल क प्रतनधत्व करत है Gzip संग्रह बनने य नकलने के लए इसक उपयग करें.
type: docs
weight: 210
url: /hi/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

यह वर्ग gzip संग्रह फ़ाइल का प्रतिनिधित्व करता है। Gzip संग्रह बनाने या निकालने के लिए इसका उपयोग करें.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`GzipArchive` संपीड़ित करने के लिए तैयार वर्ग . |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | का एक नया उदाहरण प्रारंभ करता है`GzipArchive` डीकंप्रेसिंग के लिए तैयार वर्ग। |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | का एक नया उदाहरण प्रारंभ करता है`GzipArchive` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | मूल फ़ाइल का नाम. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | अप्रबंधित संसाधनों को मुक्त करने, जारी करने या रीसेट करने से संबंधित एप्लिकेशन-परिभाषित कार्य करता है। |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | संग्रह को प्रदान की गई स्ट्रीम में निकालता है। |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | निष्कर्षण के लिए संग्रह खोलता है और संग्रह सामग्री के साथ एक स्ट्रीम प्रदान करता है. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | संग्रह को प्रदान की गई स्ट्रीम में सहेजता है। |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है। |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है। |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है। |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है। |

### टिप्पणियों

Gzip कम्प्रेशन एल्गोरिथम DEFLATE एल्गोरिथम पर आधारित है, जो LZ77 और हफमैन कोडिंग का एक संयोजन है।

### यह सभी देखें

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* नाम स्थान [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* सभा [Aspose.Zip](../../)


