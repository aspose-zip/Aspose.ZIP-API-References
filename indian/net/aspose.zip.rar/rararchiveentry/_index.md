---
title: Class RarArchiveEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Rar.RarArchiveEntry कक्ष. संग्रह के भतर एकल फ़इल क प्रतनधत्व करत है
type: docs
weight: 320
url: /hi/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | निर्माण तिथि और समय प्राप्त करता है। |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि प्रविष्टि निर्देशिका का प्रतिनिधित्व करती है या नहीं। |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | अंतिम पहुंच दिनांक और समय प्राप्त करता है. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | अंतिम संशोधित दिनांक और समय प्राप्त करता है। |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | संग्रह के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | मूल फ़ाइल का आकार प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | प्रदान की गई स्ट्रीम की प्रविष्टि निकालता है. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | दिए गए पथ द्वारा फाइल सिस्टम में प्रवेश को निकालता है। |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | निष्कर्षण के लिए प्रविष्टि खोलता है और विघटित प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |

## आयोजन

| नाम | विवरण |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | अपरिष्कृत धारा के एक हिस्से को निकाले जाने पर बढ़ता है। |

### टिप्पणियों

कास्ट ए`RarArchiveEntry` उदाहरण के लिए[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) यह निर्धारित करने के लिए कि प्रविष्टि एन्क्रिप्ट की गई है या नहीं.

### यह सभी देखें

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* नाम स्थान [Aspose.Zip.Rar](../../aspose.zip.rar/)
* सभा [Aspose.Zip](../../)


