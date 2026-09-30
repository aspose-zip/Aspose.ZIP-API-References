---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchiveEntry मेथड। निष्कर्षण के लिए प्रविष्टि को खोलता है और प्रविष्टि की सामग्री के साथ एक स्ट्रीम प्रदान करता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।

```csharp
public Stream Open()
```

### रिटर्न वैल्यू

एक पठनीय स्ट्रीम जो निकाली गई प्रविष्टि डेटा को समाहित करती है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| NotSupportedException | प्रविष्टि एक सॉलिड Apple Archive से संबंधित है या असमर्थित कम्प्रेशन विधि का उपयोग करती है। |
| InvalidDataException | प्रविष्टि के लिए संग्रहीत चेकसम या डाइजेस्ट निकाले गए डेटा से मेल नहीं खाता। |
| InvalidOperationException | प्रविष्टि एक ऐसी आर्काइव से संबंधित है जो संयोजन के लिए तैयार की गई है, या प्रविष्टि डेटा को गैर-सीक करने योग्य आर्काइव स्ट्रीम से नहीं खोला जा सकता। |
| ObjectDisposedException | स्रोत स्ट्रीम को नष्ट कर दिया गया है। |
| IOException | एक I/O त्रुटि हुई। |

## टिप्पणियाँ

वापसी की गई स्ट्रीम से पढ़ें ताकि मूल प्रविष्टि सामग्री प्राप्त हो सके। यदि आर्काइव में चेकसम फ़ील्ड हैं, तो पढ़ते समय चेकसम की जाँच की जाती है।

### संबंधित देखें

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


