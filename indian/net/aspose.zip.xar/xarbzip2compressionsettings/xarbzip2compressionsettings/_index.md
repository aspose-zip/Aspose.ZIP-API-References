---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarBzip2CompressionSettings कंस्ट्रक्टर। XarBzip2CompressionSettings क्लास का एक नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

[`XarBzip2CompressionSettings`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| blockSize | Int32 | ब्लॉक आकार सौ किलोबाइट में। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentOutOfRangeException | ब्लॉक आकार 1 और 9 के बीच नहीं है। |

## उदाहरण

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### संबंधित देखें

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

[`XarBzip2CompressionSettings`](../) क्लास का एक नया उदाहरण डिफ़ॉल्ट ब्लॉक आकार के साथ प्रारंभ करता है, जो 9 सौ किलोबाइट के बराबर है।

```csharp
public XarBzip2CompressionSettings()
```

### संबंधित देखें

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


