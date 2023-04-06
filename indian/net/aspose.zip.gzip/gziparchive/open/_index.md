---
title: GzipArchive.Open
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: GzipArchive तरक. नष्कर्षण के लए संग्रह खलत है और संग्रह समग्र के सथ एक स्ट्रम प्रदन करत है.
type: docs
weight: 50
url: /hi/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

निष्कर्षण के लिए संग्रह खोलता है और संग्रह सामग्री के साथ एक स्ट्रीम प्रदान करता है.

```csharp
public Stream Open()
```

### प्रतिलाभ की मात्रा

स्ट्रीम जो संग्रह की सामग्री का प्रतिनिधित्व करती है।

### टिप्पणियों

फ़ाइल की मूल सामग्री प्राप्त करने के लिए स्ट्रीम से पढ़ें। उदाहरण अनुभाग देखें.

### उदाहरण

आर्काइव को एक्सट्रेक्ट करता है और एक्सट्रेक्टेड कंटेंट को फाइल स्ट्रीम में कॉपी करता है।

आप .NET 4.0 और उच्चतर के लिए Stream.CopyTo पद्धति का उपयोग कर सकते हैं:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
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

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)


