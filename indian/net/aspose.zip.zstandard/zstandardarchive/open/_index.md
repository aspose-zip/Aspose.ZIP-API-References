---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZstandardArchive मेथड। निष्कर्षण के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है"
type: docs
weight: 50
url: /hi/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

अभिलेख को निकालने के लिए खोलता है और अभिलेख सामग्री के साथ एक स्ट्रीम प्रदान करता है।

```csharp
public Stream Open()
```

### रिटर्न वैल्यू

आर्काइव की सामग्री को दर्शाने वाला स्ट्रीम।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

स्ट्रीम से पढ़ें ताकि फ़ाइल की मूल सामग्री प्राप्त हो सके। उदाहरण अनुभाग देखें।

## उदाहरण

आर्काइव को एक्सट्रैक्ट करता है और एक्सट्रैक्टेड सामग्री को फ़ाइल स्ट्रीम में कॉपी करता है।

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

.NET 4.0 और उससे ऊपर के लिए आप Stream.CopyTo मेथड का उपयोग कर सकते हैं:

```csharp
unpacked.CopyTo(extracted);
```

### संबंधित देखें

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


