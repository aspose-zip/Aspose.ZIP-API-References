---
title: Bzip2Archive.Open
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2Archive तरक. नष्कर्षण के लए संग्रह खलत है और संग्रह समग्र के सथ एक स्ट्रम प्रदन करत है.
type: docs
weight: 40
url: /hi/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

निष्कर्षण के लिए संग्रह खोलता है और संग्रह सामग्री के साथ एक स्ट्रीम प्रदान करता है.

```csharp
public Stream Open()
```

### प्रतिलाभ की मात्रा

स्ट्रीम जो संग्रह की सामग्री का प्रतिनिधित्व करती है।

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
Stream decompressed = archive.Open();
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)


