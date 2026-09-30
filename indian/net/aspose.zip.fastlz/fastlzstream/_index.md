---
title: "क्लास FastLZStream"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Aspose.Zip.FastLZ.FastLZStream क्लास। एक स्ट्रीम रैपर जो FastLZ के साथ डेटा को संपीड़ित करता है। डेकोरेटर पैटर्न को लागू करता है।"
type: docs
weight: 500
url: /hi/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

एक स्ट्रीम रैपर जो डेटा को FastLZ के साथ संपीड़ित करता है। डेकोरेटर पैटर्न को लागू करता है।

```csharp
public class FastLZStream : Stream
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | `FastLZStream` क्लास का एक नया इंस्टेंस प्रारंभ करता है जो संपीड़न के लिए तैयार है। |

## प्रॉपर्टीज़

| नाम | विवरण |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि वर्तमान स्ट्रीम पढ़ने का समर्थन करता है या नहीं। |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि वर्तमान स्ट्रीम सीकिंग का समर्थन करता है या नहीं। |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि वर्तमान स्ट्रीम लिखने का समर्थन करता है या नहीं। |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | स्ट्रीम की लंबाई बाइट्स में प्राप्त करता है। |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | वर्तमान स्ट्रीम के भीतर स्थिति प्राप्त करता है या सेट करता है। |

## मेथड्स

| नाम | विवरण |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | वर्तमान स्ट्रीम को बंद करता है और वर्तमान स्ट्रीम से जुड़े किसी भी संसाधन (जैसे सॉकेट और फ़ाइल हैंडल) को मुक्त करता है। |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | इस स्ट्रीम के सभी बफ़र्स को साफ़ करता है और किसी भी बफ़र किए गए डेटा को अंतर्निहित डिवाइस पर लिखवाता है। |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | स्ट्रीम से बाइट्स की एक श्रृंखला पढ़ता है और पढ़े गए बाइट्स की संख्या के अनुसार स्ट्रीम में स्थिति को आगे बढ़ाता है। समर्थित नहीं है। |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | वर्तमान स्ट्रीम के भीतर स्थिति सेट करता है। |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | वर्तमान स्ट्रीम की लंबाई सेट करता है। |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | संपीड़ित स्ट्रीम में बाइट्स की एक श्रृंखला लिखता है और लिखे गए बाइट्स की संख्या के अनुसार इस स्ट्रीम में वर्तमान स्थिति को आगे बढ़ाता है। |

### संबंधित देखें

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


