---
title: ParallelOptions.AvailableMemorySize
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ParallelOptions संपत्त. डस्क पर स्वैप कए बन संपड़त प्रवष्टयं क समयजत करने के लए उपलब्ध मेगबइट्स में स्मृत अनुमन प्रप्त य सेट करत है यह मन केवल तभ समझ में आत हैParallelCompressInMemory सेटंग चलू हैAuto मड.
type: docs
weight: 20
url: /hi/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

डिस्क पर स्वैप किए बिना संपीड़ित प्रविष्टियों को समायोजित करने के लिए उपलब्ध मेगाबाइट्स में स्मृति अनुमान प्राप्त या सेट करता है। यह मान केवल तभी समझ में आता है[`ParallelCompressInMemory`](../parallelcompressinmemory/) सेटिंग चालू हैAuto मोड.

```csharp
public int AvailableMemorySize { get; set; }
```

### टिप्पणियों

इस मान का उपयोग प्रविष्टि के सबसे बड़े आकार की गणना करने के लिए किया जाता है जिसे दूसरों के समानांतर संकुचित किया जा सकता है। परिकलित थ्रेशोल्ड से ऊपर की सभी प्रविष्टियां क्रमिक रूप से कंप्रेस की जाएंगी. इसे रखना सुरक्षित है`AvailableMemorySize` संपत्ति जितनी बड़ी मुफ्त रैम और उससे भी बड़ी। डिफ़ॉल्ट रूप से यह माना जाता है कि आपके पास कम से कम 200 एमबी प्रति सीपीयू कोर है।

### यह सभी देखें

* class [ParallelOptions](../)
* नाम स्थान [Aspose.Zip.Saving](../../paralleloptions/)
* सभा [Aspose.Zip](../../../)


