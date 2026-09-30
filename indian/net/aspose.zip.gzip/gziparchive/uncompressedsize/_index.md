---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "GzipArchive प्रॉपर्टी। मूल फ़ाइल का आकार प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

मूल फ़ाइल का आकार प्राप्त करता है।

```csharp
public ulong UncompressedSize { get; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

डिकम्प्रेशन के दौरान, यह प्रॉपर्टी गलत आकार रख सकती है। यदि अनकम्प्रेस्ड फ़ाइल का आकार 4GB से अधिक हो जाता है, तो हेडर में 32-बिट सीमा के कारण यह प्रॉपर्टी गलत मान देगी।

### संबंधित देखें

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


