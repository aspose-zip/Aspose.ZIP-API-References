---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarArchive मेथड। एंट्री सूची से किसी विशिष्ट एंट्री की पहली उपस्थिति को हटाता है"
type: docs
weight: 50
url: /hi/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

एंट्री सूची से किसी विशिष्ट एंट्री की पहली उपस्थिति को हटाता है।

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| एंट्री | XarEntry | एंट्री सूची से हटाने के लिए एंट्री। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *entry* शून्य है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए खुला नहीं है। |

## उदाहरण

यहाँ बताया गया है कि आप अंतिम एंट्री को छोड़कर सभी एंट्री कैसे हटाएँ:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### संबंधित देखें

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


