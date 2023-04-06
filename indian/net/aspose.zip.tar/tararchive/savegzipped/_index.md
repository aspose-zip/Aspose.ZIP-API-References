---
title: TarArchive.SaveGzipped
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. gzip कम्प्रेशन के सथ संग्रह क स्ट्रम में सहेजत है.
type: docs
weight: 130
url: /hi/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

gzip कम्प्रेशन के साथ संग्रह को स्ट्रीम में सहेजता है.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
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

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

आर्काइव को फ़ाइल में gzip कम्प्रेशन के साथ पथ द्वारा सहेजता है.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
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
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


