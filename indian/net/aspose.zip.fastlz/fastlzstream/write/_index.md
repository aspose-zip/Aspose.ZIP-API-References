---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "FastLZStream मेथड। बाइट्स की एक श्रृंखला को संपीड़न स्ट्रीम में लिखता है और इस स्ट्रीम में वर्तमान स्थिति को लिखे गए बाइट्स की संख्या से आगे बढ़ाता है"
type: docs
weight: 120
url: /hi/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

संपीड़ित स्ट्रीम में बाइट्स की एक श्रृंखला लिखता है और लिखे गए बाइट्स की संख्या के अनुसार इस स्ट्रीम में वर्तमान स्थिति को आगे बढ़ाता है।

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| बफ़र | Byte[] | बाइट्स का एक एरे। यह मेथड बफ़र से वर्तमान स्ट्रीम में count बाइट्स कॉपी करता है। |
| offset | Int32 | बफ़र में शून्य-आधारित बाइट ऑफ़सेट जहाँ से वर्तमान स्ट्रीम में बाइट्स कॉपी करना शुरू किया जाता है। |
| count | Int32 | वर्तमान स्ट्रीम में लिखे जाने वाले बाइट्स की संख्या। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | यदि स्ट्रीम को डिस्पोज़ किया गया हो तो फेंका जाता है। |
| ArgumentNullException | *buffer* `null` है। |

### संबंधित देखें

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


