---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "SevenZipEntrySettings प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त या सेट करता है कि क्या एंट्रीज़ को जोड़कर एकल डेटा ब्लॉक के रूप में माना जाए"
type: docs
weight: 50
url: /hi/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

एंट्रीज़ को जोड़ने और उन्हें एकल डेटा ब्लॉक के रूप में मानने के लिए संकेत करने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool Solid { get; set; }
```

## टिप्पणियाँ

आर्काइव निर्माण के समय सॉलिड 7z आर्काइव के लिए `SevenZipEntrySettings` प्रदान करें।

## उदाहरण

निम्न उदाहरण दर्शाता है कि कैसे एक डायरेक्टरी को बिना एन्क्रिप्शन के LZMA2 संपीड़न के साथ सॉलिड 7z आर्काइव में संकुचित किया जाए।

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### संबंधित देखें

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


