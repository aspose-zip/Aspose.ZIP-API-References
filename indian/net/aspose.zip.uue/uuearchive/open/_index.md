---
title: "UueArchive.Open"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "UueArchive मेथड। डिकोडिंग के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है"
type: docs
weight: 60
url: /hi/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

डिकोडिंग के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है।

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

उपयोग:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 और उससे ऊपर - Stream.CopyTo मेथड का उपयोग करें:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 और पहले - बाइट्स को मैन्युअल रूप से कॉपी करें:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


