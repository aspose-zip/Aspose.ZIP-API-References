---
title: TarArchive.SaveZCompressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. आर्कइव क जेड कम्प्रेशन के सथ स्ट्रम में सेव करत है
type: docs
weight: 160
url: /hi/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

आर्काइव को जेड कम्प्रेशन के साथ स्ट्रीम में सेव करता है।

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *output* शून्य है। |
| ArgumentException | *output* लिखने योग्य नहीं है। |

### टिप्पणियों

*output*लिखने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
        }
    }
}
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

आर्काइव को जेड कम्प्रेशन के साथ पाथ बाई पाथ में सेव करता है।

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |

### उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


