---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ArchiveFactory मेथड। प्रदान किए गए अभिलेख प्रारूप का उपयोग करके निर्दिष्ट निर्देशिका को अभिलेख फ़ाइल में संकुचित करता है"
type: docs
weight: 10
url: /hi/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

प्रदान किए गए अभिलेख प्रारूप का उपयोग करके निर्दिष्ट निर्देशिका को अभिलेख फ़ाइल में संकुचित करता है।

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | संकुचित की जाने वाली निर्देशिका का पथ। |
| outputFileName | String | गंतव्य फ़ाइल नाम। |
| archiveFormat | ArchiveFormat | बनाने के लिए अभिलेख का प्रारूप (जैसे, zip, rar, tar, आदि)। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| DirectoryNotFoundException | *path* द्वारा निर्दिष्ट निर्देशिका मौजूद नहीं होने पर फेंका जाता है। |
| ArgumentException | *path* null या खाली स्ट्रिंग होने पर फेंका जाता है। |
| NotSupportedException | निर्दिष्ट *archiveFormat* असमर्थित या अज्ञात होने पर फेंका जाता है। |
| ArgumentNullException | *path* `null` है। |

## टिप्पणियाँ

यह मेथड *path* पैरामीटर द्वारा निर्दिष्ट स्थान पर एक अभिलेख फ़ाइल बनाएगा। अभिलेख फ़ाइल का नाम आमतौर पर निर्देशिका नाम के बाद *archiveFormat* के आधार पर उपयुक्त फ़ाइल एक्सटेंशन होगा। निर्देशिका स्वयं संशोधित या हटाई नहीं जाएगी।

## उदाहरण

यहाँ CompressDirectory मेथड का उपयोग करने का एक उदाहरण है:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// यह निर्दिष्ट पथ पर डायरेक्टरी की सामग्री के साथ एक ZIP फ़ाइल बनाएगा।
```

### संबंधित देखें

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


