---
title: Class ArchiveEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.ArchiveEntry कक्ष. संग्रह के भतर एकल फ़इल क प्रतनधत्व करत है
type: docs
weight: 20
url: /hi/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | संग्रह के भीतर प्रविष्टि की टिप्पणी प्राप्त करता है। |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | कंप्रेशन या डिकंप्रेशन के लिए सेटिंग प्राप्त करता है. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि प्रविष्टि निर्देशिका का प्रतिनिधित्व करती है या नहीं। |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | अंतिम संशोधित तिथि और समय प्राप्त या सेट करता है। |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | संग्रह के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | मूल फ़ाइल का आकार प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | प्रदान की गई स्ट्रीम की प्रविष्टि निकालता है. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | दिए गए पथ द्वारा फाइल सिस्टम में प्रवेश को निकालता है। |
| [Open](../../aspose.zip/archiveentry/open/)(string) | निष्कर्षण के लिए प्रविष्टि खोलता है और विघटित प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |

## आयोजन

| नाम | विवरण |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | अपरिष्कृत धारा के एक हिस्से के संकुचित होने पर उठता है। |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | अपरिष्कृत धारा के एक हिस्से को निकाले जाने पर बढ़ता है। |

### टिप्पणियों

कास्ट ए`ArchiveEntry` उदाहरण के लिए[`ArchiveEntryEncrypted`](../archiveentryencrypted/) यह निर्धारित करने के लिए कि प्रविष्टि एन्क्रिप्ट की गई है या नहीं.

### यह सभी देखें

* interface [IArchiveFileEntry](../iarchivefileentry/)
* नाम स्थान [Aspose.Zip](../../aspose.zip/)
* सभा [Aspose.Zip](../../)


