---
title: TarEntry.Open
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarEntry तरक. नष्कर्षण के लए प्रवष्ट खलत है और प्रवष्ट समग्र के सथ एक स्ट्रम प्रदन करत है
type: docs
weight: 50
url: /hi/net/aspose.zip.tar/tarentry/open/
---
## TarEntry.Open method

निष्कर्षण के लिए प्रविष्टि खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।

```csharp
public Stream Open()
```

### प्रतिलाभ की मात्रा

धारा जो प्रविष्टि की सामग्री का प्रतिनिधित्व करती है।

### टिप्पणियों

फ़ाइल की मूल सामग्री प्राप्त करने के लिए स्ट्रीम से पढ़ें। उदाहरण अनुभाग देखें.

### उदाहरण

उपयोग:

.NET 4.0 और उच्चतर - Stream.CopyTo पद्धति का उपयोग करें:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 और पहले - मैन्युअल रूप से बाइट कॉपी करें:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### यह सभी देखें

* class [TarEntry](../)
* नाम स्थान [Aspose.Zip.Tar](../../tarentry/)
* सभा [Aspose.Zip](../../../)


