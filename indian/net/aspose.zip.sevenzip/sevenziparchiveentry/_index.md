---
title: Class SevenZipArchiveEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry कक्ष. 7z संग्रह के भतर एकल फ़इल क प्रतनधत्व करत है
type: docs
weight: 670
url: /hi/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

7z संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | कंप्रेशन या डिकंप्रेशन के लिए सेटिंग प्राप्त करता है. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि प्रविष्टि निर्देशिका का प्रतिनिधित्व करती है या नहीं। |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | अंतिम संशोधित दिनांक और समय प्राप्त करता है। |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | संग्रह के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | मूल फ़ाइल का आकार प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | प्रदान की गई स्ट्रीम की प्रविष्टि निकालता है. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | दिए गए पथ द्वारा फाइल सिस्टम में प्रवेश को निकालता है। |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | निष्कर्षण के लिए प्रविष्टि खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |

## आयोजन

| नाम | विवरण |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | अपरिष्कृत धारा के एक हिस्से के संकुचित होने पर उठता है। |

### टिप्पणियों

कास्ट ए`SevenZipArchiveEntry` उदाहरण के लिए[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) यह निर्धारित करने के लिए कि प्रविष्टि एन्क्रिप्ट की गई है या नहीं.

### यह सभी देखें

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* नाम स्थान [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* सभा [Aspose.Zip](../../)


